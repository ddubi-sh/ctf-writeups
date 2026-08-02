# picoCTF - MY GIT

## Challenge

- Category: General Skills
- Topic: Git, Git metadata, remote repository
- Difficulty: Easy
- Platform: picoCTF

## Description

`flag.txt`를 특정 Git 사용자 정보로 커밋하고 원격 저장소에 push하여 플래그를 획득하는 문제다.

문제에서 제공된 핵심 문구:

> Only flag.txt pushed by root:root@picoctf will be updated with the flag.

## Key Idea

Git 커밋에는 파일 변경사항뿐 아니라 작성자 이름과 이메일도 메타데이터로 저장된다.

따라서 Git 사용자 정보를 다음과 같이 설정해야 한다.

```bash
git config user.name "root"
git config user.email "root@picoctf"
