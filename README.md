# One Week One Code Review

## 1주에 1번씩 서로 공부한 코드를 리뷰 해주며, 성장하기 위한 레포지토리 입니다.

## 어떤것을 올려야 하나요?

어떤것이든 좋습니다. 언어도 좋고, 라이브러리도 좋습니다. 마트다운으로 공부한 내용을 정리해도 좋습니다.

1주에 1회 이상 커밋을 하고, 풀 리퀘스트만 보내면 됩니다.

## Rule

### Pull Requests

- main Branch 에는 아무도 푸시할 수 없습니다.
무조건 풀 리퀘스트를 통해서만 main branch 수정이 가능합니다.
- 각자 이름/공부하는 내용 의 branch 를 생성합니다.
ex) jeongtae/scala_spark
- 각자 이름의 폴더도 생성합니다.
jeongtae/
- 공부한 내용은 모두 자신의 이름의 폴더 안에서 업데이트 합니다.
- 이상한 파일이 같이 커밋되지 않게 설정해주세요 `.gitignore`
- 커밋 컨벤션을 최대한 맞춰주세요.
- 1주간 공부를 진행한 뒤 마음에 드는 사람을 리뷰어로 지정해(1명 이상) 풀리퀘스트를 보냅니다.

### Reviewer

- 공부한 내용 외의 파일이 올라온 경우 커멘트 후 close
- 파이썬으로 코드를 작성한 경우 `PEP8`포맷을 검사합니다.
⇒ 지키지 않았으면 과감히 close
- 공부한 내용을 읽어보고 느낀점을 적어줍니다! + merge!
- 머지한 이후에는 머지된 브랜치를 삭제해줍니다.
ex) jeongtae/scala_spark 삭제

### example rule

```bash
git clone git@github.com:OwO-CR/OWOCR.git
cd OWOCR/

mkdir jeongtae/
touch jeongtae/first_file.sc
echo "val firstFile: Int = 1" >> jeongtae/first_file.md

git branch jeongtae/scala_spark
git checkout jeongtae/scaal_spark

git add jeongtae/first_file.sc
git commit -m "Init: first commit"

git push origin jeongtae
```

이후에 깃허브로 이동해 리뷰어를 설정하고 main 브랜치에 PR!
