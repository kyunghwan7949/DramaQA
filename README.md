# DramaQA Knowledge Graph Generation


script(AnotherMissOh_script.json) / input_paths(AnotherMissOhQA_train/val/test_set.json) 데이터셋 경로 수정 필요


### 도커 코드, 이미지 및 가상환경
```bash
docker pull kyunghwan7949/dramaqa:latest
docker run -it --gpus '"device=2"' --ipc=host --name dramaqa docker.io/kyunghwan7949/dramaqa:latest /bin/bash
conda activate dramaqa
cd /dramaqa
```
 
### 초기 폴더 생성 및그래프 생성  
```bash
bash download_raw_data.sh
python preprocess.py 
``` 
  
  
 
 
 
