# Segmentation

## 1. VOC_Loader
로더가 하는 일은 

loader enumerate 한번에, 원본 이미지 파일과 class segmentation 파일들을 배치 개수만큼 읽어와서

augmentation, crop, shrink, pad를 진행한 후

결과 img(N, C, H, W), seg(N, H, W)와 pad 값을 namedtuple로 출력한다. 
