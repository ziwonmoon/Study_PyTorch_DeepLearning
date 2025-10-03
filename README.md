# Study_PyTorch_DeepLearning
"딥 러닝 파이토치 교과서 - 입문부터 LLM 파인튜닝까지" 실습 공간

본 리포는 "딥 러닝 파이토치 교과서 - 입문부터 LLM 파인튜닝까지"(Bryce and Eddie, wikidocs, https://wikidocs.net/book/2788)의 실습 결과와 개인적인 추가 코드로 이루어져 있습니다.

## 중요 개념 & 햇갈리는 개념 정리

### 텐서
n차원으로 구성된 배열 <br>
ex. <br>
벡터 = 1차원 텐서 <br>
행렬 = 2차원 텐서 <br>
3차원 이상 : 3차원 텐서, 4차원 텐서... <br>

![2D 텐서 설명 이미지](docs/images/2d_tensor_image.jpeg)
2차원 텐서의 경우, (행렬로 치면) 행의 크기 : batch size, 열의 크기 : dim



비전 분야와 자연어 분야의 텐서 차원별 네이밍이 다르다.

###### 3D텐서 - 비전에서
|t|=(batch size, widht, height) <br>
![3D 텐서 (비전) 설명 이미지](docs/images/3d_tensor_Vision.jpeg)


###### 3D텐서 - NLP에서 
![3D 텐서 (NLP) 설명 이미지](docs/images/3d_tensor_NLP.jpeg)