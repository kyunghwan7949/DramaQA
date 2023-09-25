# DramaQA Knowledge Graph 생성 코

## TGB baseline 코드
```bash
script(AnotherMissOh_script.json) / input_paths(AnotherMissOhQA_train/val/test_set.json) 데이터셋 경로 수정 필요
```

## 도커 이미지 및 가상환경
- 72/230 서버는 세팅완료
```bash
docker pull kyunghwan7949/dramaqa:latest
docker run -it --gpus '"device=2"' -v /media:/data -v /home/:/mount -v --ipc=host --name dramaqa docker.io/kyunghwan7949/dramaqa:latest /bin/bash
conda activate qagnn
```

## Train
```bash
python preprocess.py
```
