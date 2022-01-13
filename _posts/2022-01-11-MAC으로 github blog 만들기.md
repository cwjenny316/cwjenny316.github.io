---
layout: post
title:  "GITHUB BLOG 만들기"
date:   2015-04-18T14:25:52-05:00
author: JEN
categories: TIL
tags:	jekyll
cover:  "/assets/instacode.png"
---

## MAC 초보 사용자의 github.io 블로그 오픈

대부분의 프로세스는
[Zedd0202][refBlog]님의 블로그를 참조해서 만들었습니다.. 초보 MAC 사용자에게는 만들면서 여러 난항이 있었는데...



### 1. GITHUB BLOG 주소 설정

github.io 블로그를 만들려면, repository 주소를 반드시 [Username]/[username.github.io] 로 설정해야 합니다.
예를 들어 , git username이 Korea 라면 맞는 주소는 아래와 같습니다.
  - Korea.github.io (O)
  - korea.github.io (X)
  - hi.github.io (X)

-> 해결 : 저의 경우, username 과 다른 주소를 넣어 블로그가 만들어지지 않았고.. 또 하나..

  - git repository 생성 시 반드시 public repository로 생성하셔야 합니다 (private github.io 는 유료)

이것때문에 쓸데없이 시간을 잡아먹었습니다 ㅎㅎ







### 2. GIT CLONE 시 터미널에서 github 로그인
Git Clone 시 터미널에서 로그인을 해야합니다.
github 아이디/비밀번호로 로그인 했을 시, Access Denied 나, Authentication Failed 와 같은 메시지가 떴었습니다;;

-> 해결 : Persoanl Access Token  생성하고 해당 토큰을 비밀번호로 로그인

github 업데이트 이후로, 로그인 할 시 personal access token 이 필요하다고 합니다.
아이디 비밀번호를 아이디/token으로 해주니 해결되었습니다.




### 3. 생소한 git 터미널 명령어
구글링을 통해 명령어를 익혔습니다.
git에서 주로 쓰는 명령어는 아래와 같습니다.

1) 파일 커밋 및 push
{% highlight javascript %}
—git add all
—git commit -, “write commit message”
—git pust -u origin main"
{% endhighlight %}

2) 빈 파일 커밋
{% highlight javascript %}
git commit --allow-empty -m "Trigger notification"
{% endhighlight %}


### 마치며
이상 많은 시행착오를 거쳐 블로그를 만들었고, 블로그의 기록 뿐만 아니라 댓글, 메뉴정렬 등 기타 기능도 구현해보고자 합니다.



[refBlog]:      https://zeddios.tistory.com/1222?category=682196
