## github에 git bash 터미널에 설정되어 있는 계정 변경하기.

1. git bash 창을 연다.

2. 현제 git bash에 설정되어 있는 터미널 계정을 확인해 본다.
```cmd
$ git config user.name
```

```
$ git config user.email
```

3. 계정 바꾸기
```
$ git config --global user.name 바꿀 계정이름
```
```
$ git config --global user.email 바꿀 이메일
```

'바꿈 완료!'
