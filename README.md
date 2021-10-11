# MiD (Medical Image Deep Learning Framework)


### 1. pip install MiD
- 패키지 다운로드


### 2. Data Organizer
- 포멧에 맞게 데이터 수정
- Path를 입력하면 자동으로 저장
- Data_Organizer의 생성자에는 저장 주소와 파일 이름 앞에 붙을 ID를 넣는다
- run에는 각각 저장할 Label 데이터의 주소와 Image 데이터 주소를 넣는데, 이 때 이미지 주소는 Multi-modal 지원을 위해 List 형식으로 넣음.

    from mid.data_organizer import Data_Organizer
    
    TR_LOAD_PATH = os.path.join(LOAD_PATH, 'imagesTr')
    SEG_LOAD_PATH = os.path.join(LOAD_PATH, 'labelsTr')


    img_file = [e for e in os.listdir(TR_LOAD_PATH) if e[0] != '.']
    seg_file = [e for e in os.listdir(SEG_LOAD_PATH) if e[0] != '.']

    
    img_file = sorted(img_file)
    seg_file = sorted(seg_file)

    
    organizer = Data_Organizer(SAVE_PATH, 'Task04_Hippocampus')



    for i in range(len(img_file)):
        seg_file_path = os.path.join(SEG_LOAD_PATH, seg_file[i])
        img_file_path = os.path.join(TR_LOAD_PATH, img_file[i])
        organizer.run(seg_file_path, [img_file_path], i)
