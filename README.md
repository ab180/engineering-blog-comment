# AB180 Engineering Blog Comments

[AB180 기술 블로그](https://engineering.ab180.co/)의 댓글을 보관하는 저장소입니다. [Utterances](https://utteranc.es/)가 GitHub Issues를 댓글 저장소로 사용합니다.

## 댓글 저장 구조

1. 블로그 글을 열면 Utterances가 글의 URL 경로(`pathname`)에 해당하는 Issue를 찾습니다.
2. 연결된 Issue가 없는 글에 첫 댓글이 등록되면 `utterances-bot`이 Issue를 만듭니다.
3. 이후 댓글은 그 Issue의 댓글로 저장되며 블로그와 GitHub에서 확인할 수 있습니다.

예를 들어 `stories/standardizing-alert-system-with-iac` 글의 댓글은 같은 경로를 제목으로 가진 Issue에 저장됩니다.

## 운영

댓글 데이터는 이 저장소의 **Issues** 탭에 있습니다. 소스 파일과 코드의 마지막 push 날짜로 댓글 사용 여부를 판단하지 않습니다.

블로그는 Oopy에서 Utterances를 연결합니다. 저장소 이름을 바꿀 때는 Oopy의 Utterances `repo` 설정도 함께 갱신합니다. 댓글을 보존하려면 저장소와 Issues를 유지해야 합니다.
