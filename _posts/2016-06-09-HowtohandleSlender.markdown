---
layout: post
title:  "Modify Slender Theme"
color:  black
width:   3
height:  1
date:   2016-06-05 00:00:00 +0900
categories: jekyll update
---
### Introduction

지금까지 Github+Jekyll을 통해 홈페이지를 구성해왔다. 이제 마지막으로 꾸밀 일만 남았다. 하나하나 파일들을 살펴보며 Static Blog를 내것으로 만들어보자.

#### First of all - Theme setting

Github+Jekyll을 통해 blog를 구성하고 난 후 theme를 설정하자. 모든 내용은 Slender theme에 적용되며, 기타 다른 테마에는 적용되지 않을 수 있다.

- 인터넷에서 원하는 theme를 받는다.
- 기존 생성된 blog의 모든 파일을 지운다.
- Theme에 있는 모든 파일을 blog에 새로 복사한다.
- ./_config.yml를 다음과 같이 변경
{% highlight markdown %}
baseurl: "/jekyll-slender-template"
baseurl: ""
{% endhighlight %}
- 위에 처럼 코드 highlight를 적용하고 싶다면, 홈페이지 제작자가 제공한 소스를 열어보자.

### Part 1. Layouts

#### Modify ./_config.yml

이 파일은 모든 테마에 공통적으로 있는 파일이다. Configration, 말 그대로 배열, 배치와 같은 모든 설정을 여기서 담당한다. 바로 파일을 열어 한번 살펴보자.
{% highlight markdown %}
# Site settings
title: My Portfolio
email: your-email@domain.com
description: > # this means to ignore newlines until "baseurl:"
  Jannik Richter, jannik811@gmail.com
baseurl: "" # the subpath of your site, e.g. /blog
url: "http://yourdomain.com" # the base hostname & protocol for your site
twitter_username: jekyllrb
github_username:  jekyll

# Build settings
markdown: kramdown
{% endhighlight %}

- Title
    + title의 My Portfolio라는 것이 어디에 적용되어 있는가? 초기 테마에서, 맨 위 빨간 바탕에 적혀있을 것이다.
    + 바꾸고 나면 뭔가 글씨가 바뀐다.
    + 나는 '기승전 딥러닝'을 외치는 사람이라, 'Introduction, Development, Turn and Deeplearning'으로 하였다.
    + 여기 한글로 쓰면 에러난다, 짜증나지만 영어쓰자.
- email 뭔지 알겠지..
- url은 첫시간에 얘기한 너님들이 신청한 domain을 여기에 넣어주면 된다.
    + 그러면, 인터넷에 domain을 입력하면 여기로 redirection된다.
- twitter, github username : 입력해라. 안해도된다 물론, 심지어 주석처리해도 된다.
- _config.yml의 윗부분 주석을 읽어보자.

{% highlight markdown %}
# For technical reasons, this file is *NOT* reloaded automatically when you use
# 'jekyll serve'. If you change this file, please restart the server process.
{% endhighlight %}
- 해석이 되는가. 음, 해석하면, _config.yml은 수정을 하고나면 기술적인 문제 때문에 어쩔 수 없이 다시 서버를 껏다 켜달라고 한다.
    + ruby on rail에서 ctrl+c를 눌러 서버를 껏다 다시 켜주면 적용된다.
    + _config.yml을 제외한 나머지 파일들은 수정할 때 그럴 필요 없다.
    + 그냥 놔두면 알아서 업데이트 된다.







### Conclusion

홈페이지 제작 강좌를 준비하며, 정말 많은 것들을 배웠다.
사실 한가지 먼저 고백하자면 나는 이 강좌를 시작하기 전에 Jekyll이나 Github를 단 한번도 써본 적이 없다.
처음엔 wordpress를 사용해서 간단한 홈페이지를 만드는 것으로 때우려고 생각했었다.
Jekyll이나 Github는 처음 접하는 사람에게 너무나 어려운 것이고, 이것을 설명할 자신조차 없었다.
하지만 1강을 준비하고, 수업하며 어중간한 것들로는 자리에 앉아있는 사람들에게 만족할만한 수업을 제공해야겠다는 생각이 들게 되었다.
지금도 1강 때, 인터넷에 대한 개념, Haroopad를 통한 Markdown문법을 설명할 때 수업을 듣는 여러분의 자세는 강사라고 서있는 나를 매우 긴장하게 했었다.
1강 쉬는 시간에 줄담배를 피우며, 준비가 부족한 것에 대한 후회를 하며 손을 부들부들 거렸다.

부족함에도 불구하고 뭔가 남는 수업을 진행하기 위해 **공부하며 가르치는** 위험한 방식을 선택했다. 
1주차가 끝난 시점부터 나는 수업을 하기 위해 여러가지를 공부했고, 나와 같이 강의한 한재윤씨는 더 많은 시간과 노력을 할애했다. 하나라도 더 좋은 것, 오래 남을 수 있는 것을 생각하니 재윤이의 Github + Jykell을 포기 할 수 없었고 이래저래 준비하여 부족한 강의를 이제 1강만 남겨두게 되었다.

아직 아쉬운 것이 많다. 더 많은 것들을 설명하고 싶었다. 
특히 수업이라는 특성은 처음부터 모든 것을 알려줘야 한다는 부담감이 있어 모든 background를 설명하고 이해시키려 하였고, 한재윤씨의 2강 역시 그런 마음으로 준비했을 것이라 생각한다.

이제 곧 마지막 4주차 수업으로 들어가면서, 지금까지의 얘기와는 전혀 다른 이야기를 하나 강조하고 싶다.

> 필요하면 그때 그때 찾아쓰기


처음부터 모든 것을 찾아서 다 마스터하고, 시작해야하지 하는 마음가짐은 여러분이 학기 중 교수님의 수업시간에 가지면 좋을 마인드이지 홈페이지를 만드는데 있어 절대로 가져서는 안되는 마인드다 (프로그래밍과 같은 컴퓨터 관련 모든 것에 해당한다). 수업을 통해 느꼈을지 모르겠지만, 컴퓨터와 관련된 분야는 특히 매우 빠르게 변화한다. 어제 내가 읽었던 report가 오늘은 구식 기술이 되어버린다. 수업과 같이 정리하고 읽는 것은 의미가 없다는 것이다. 당신이 정리해서 공부하는 동안 어딘가에서 새로운 기술이 개발되고 적용된다. 단적인 예로 이 글을 읽는 그 순간에도 어딘가에서 새로운 Jekyll theme는 개발되고, 업로드 되고, 사용될 것이다. 그러니 처음부터 정리해서 공부하려는 마음가짐 따위는 내려놓아도 된다. 그냥 필요하면 찾아서 공부를 하는 것이 최선이다. 특히 밑에서 설명하기 시작할 theme 사용법 역시 그렇다. 나도 인터넷을 뒤져가며, 그냥 필요해서 그때 찾아서 그때 적용하고 정리만 해서 강의랍시고 떠드는 것이다. 저걸 어떻게 하지 이런 마음보다는 "저 앞에 저 강사놈도 지금 설명하는 것 말고는 모르겠구나." 하는 마음으로 본인이 찾아 공부하는 습관을 들이길 바란다. 그렇게 공부한게 쌓여가면, 어느 순간 누군가가 당신에게 그 분야에 대해 도움을 요청할 것이고, 그게 쌓인다면 당신도 강단에 서서 -나 처럼 진땀을 흘려가며 - 누군가에게 당신의 지식을 알려주게 될 것이다.

히힠. 그리고 무엇보다 지금까지 믿고 따라와준 여러분께 진심으로 감사의 말을 전한다.




