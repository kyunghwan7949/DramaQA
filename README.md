# DramaQA Knowledge Graph Generation 코드


script(AnotherMissOh_script.json) / input_paths(AnotherMissOhQA_train/val/test_set.json) 데이터셋 경로 수정 필요


### 도커 이미지 및 가상환경
```bash
docker pull kyunghwan7949/dramaqa:latest
docker run -it --gpus '"device=2"' -v --ipc=host --name dramaqa docker.io/kyunghwan7949/dramaqa:latest /bin/bash
conda activate dramaqa
```

### 그래프 생성 
```bash
python preprocess.py
```
