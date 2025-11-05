# Study_PyTorch_DeepLearning
"딥 러닝 파이토치 교과서 - 입문부터 LLM 파인튜닝까지" 실습 공간<p>
본 리포는 "딥 러닝 파이토치 교과서 - 입문부터 LLM 파인튜닝까지"( Bryce and Eddie, wikidocs, https://wikidocs.net/book/2788 )의 실습 결과와 개인적인 추가 코드로 이루어져 있습니다.

## 중요 개념 & 햇갈리는 개념 정리
개념 정리 Notion 링크 : https://scrawny-author-314.notion.site/Pytorch-Deep-Learning-29b223c8e74c80e9b1f8e5ec8c5bd89d

## 환경 설정
VSCode로 Colab에 SSH 접속하여 사용하기를 고려하였으나, Colab 정책 상 무료 세션에서는 원격 사용이 금지될 수 있기 때문에, Colab Notebook을 이용하기로 하였습니다.<p>
버전 관리와 포트폴리오를 위하여 Google Drive의 파일을 Github로 푸시해야 할 필요가 있습니다. <p>
1. Colab에서 Google Drive 마운트 후에 푸시 (선택)
2. Google Drive - Local Drive 동기화 후 로컬에서 푸시 <p>
1의 방법으로는, 동기화 시간을 기다리지 않아도 되는게 장점이나, Colab Notebook 외의 파일(Markdown 등)을 편집할때 불편한게 단점입니다. <p>
2의 방법으로는, 동기화 시간을 기다려야 한다는게 단점이나, 대부분의 파일 수정을 편한 IDE로 이용할 수 있는게 장점입니다.<p>
매번 푸시하기 전에 동기화를 기다려야 한다면 실수가 일어날 수 있고 기다리기도 번거로울 수 있기 때문에 1의 방법을 택했습니다.<p>

#### Google Colab - Git Push
```Python
COMMIT_MESSAGE = """
커밋 메시지 작성
"""

from google.colab import drive
drive.mount('/content/drive')

%cd <<PATH TO PROJECT DIR>>
!git config --global user.email '<<EMAIL>>'
!git config --global user.name '<<NAME>'

!git add -A --all
!git commit -m "$COMMIT_MESSAGE"
!git push
```
#### Google Colab - Git Pull
```Python
from google.colab import drive
drive.mount('/content/drive')

%cd <<PATH TO PROJECT DIR>>

!git pull origin main
```
