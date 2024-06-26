# 버전관리 시스템

속 없는 붕어빵이 없는 것 처럼 개발자에게는 버전관리 시스템이란 땔래야 땔 수 없다. 그 중에서도 GitHub(github, Github 아님...)는 붕어빵 중에서도 팥붕어빵이라고 할 수 있다!

## 버전관리가 뭔데?
> 깃허브는 [Ruby on Rails](https://rubyonrails.org/)로 작성된 **분산 버전 관리** 툴인 깃 저장소 호스팅을 지원하는 웹 서비스이다.
>> [위키피디아 발췌](https://ko.wikipedia.org/wiki/%EA%B9%83%ED%97%88%EB%B8%8C)

깃허브는 버전관리 도구이란다...

버전관리 도구이 뭘까?

버전 관리 도구이란 파일 변화를 "시간"에 따라 기록했다가 추후 **특정 시점**의 버전을 꺼내올 수 있는 도구이란다.

즉, 현재의 코드가 문제가 생기거나 업데이트 내용의 전체적인 수정이 필요하다면 코드 전체를 수정하는것이 아닌 업데이트 이전으로 돌아갈 수 있다는 내용이다. 또한 매번 새로운 업데이트를 진행할 때마다 무엇이 추가되었고 무엇이 수정되었는지 손 쉽게 확인할 수 있다.

### 아니 그냥 로컬 파일에 일일이 다 기록해 놓으면 되는거 아니야?
개발 업무는 혼자서 진행하는 것이 아니다. 한 프로젝트를 진행할 때 여러명의 서로 다른 분야의 개발자들이 서로 다른 업무를 맡에 진행을 하게 된다. 또한 개발자들끼리만 협업하는 것이 아니라 이외의 관련 분야에 종사하시는 팀원들 또한 개발 프로젝트에 투입이 된다.

이렇듯 다양한 사람들이 함께 작업을 진행하게 되는데 업데이트를 일일이 개인 로컬 파일, 혹은 회사 내 공유 폴더에서 프로젝트를 진행하게 된다면 코드 충돌(code conflict)문제는 불 보듯이 뻔할 것이다. 이외에도 정말 다양한 이유가 있지만 잘 생각해보면 대다수의 개발자들이 분산버전관리 시스템을 통해서 프로젝트를 진행하는데는 그만한 이유가 있지 않을까?


### 'G'it'H'ub
오늘 다룰 내용은 수많은 다양한 버전 관리 도구들 중에 **GitHub** 에 대해서 간단하게 알아 보는 시간이다.

많고 많은 다양한 회사들 중에 GitHub을 알아보는 이유는...

간단하게 가장 많은 사람들이 GitHub를 통해 프로젝트를 진행중이기 때문이다!
(해당 포스팅 또한 GitHub에서 버전을 관리해가며 글을 작성중이다.)

|랭킹|회사|
|--|----------|
| 1 | GitHub |
| 2 | GitLab |
| 3 | Snowtrack |
| 4 | Simul |
| 5 | Mercurial |
| 6 | Kactus |
| 7 | Bitbucket |
| 8 | CVS |
| 9 | Unity Version Control |

[출처:logit.io](https://logit.io/blog/post/version-control-tools/)

###깃허브는 왜 쓸까?

"엥??? 내가 옆에서 애들이 뚜시따시 하면서 만지는거 봤는데~ 그거 그냥 깃헙 홈페이지 들어가서 치면 되는거 아니야???"

맞는 말이다. 쳐 맞는 말.

윗 글에서 깃허브라는 분산버전 관리 툴을 왜 쓴다고 했을까?

~~1. 그냥 다들 쓰니까 있어보일라고 (손님 진짜 맞을래요???)~~

요약하자면
```
1. 추적 관리에 용이
2. 협업시 코드 충돌 방지
3. 백업 및 복구의 편리
```

위의 세가지 이유로 분산관리 도구를 쓴다고 필자는 생각한다. (아마 대부분의 다른 개발자들도 그렇게 생각할 것이고)

#### 기본 명령어 (4가지)
1. **git pull || git clone**
2. **git add .**
3. **git commit -m '추가||수정 사항'**
4. **git push**
---

GitHub에 파일들을 끌어오거나 보낼라면 우선적으로 **어디** 라는 단어가 키워드이다.

    어디서 파일을 끌어올 것이고
    어디로 파일을 보내는지

처음 GitHub에 가입을 하게 되면 Repository라는 것을 만들어야 한다.

왜?

그래야 **어디**라는게 해결될테니까.

Repository 즉, 레포는 쉽게 얘기하면 저장소 같은 개념이다.

**Repository**에서 파일을 받아오고 **Repository**로 파일을 보낸다.

##### git clone
---
> git clone https://깃허브주소.com .
git clone : 처음 레포를 내 로컬 파일로 불러올 때 쓰이는 명령어.

말 그대로 정보를 'clone', 복제 해오는 단계이다.

레포에 닮겨있는 저장소의 정보를 받아와야 주던 받던 할 것 아닌가...

##### git add .
저장소를 연결하고 뭘 해야될까???

'음 이쁘게 잘 들어왔어! 만족!' 하고 끝낼게 아니지 않는가...

저장소의 정보를 받아왔으면 파일 안에 있는 정보를 수정하거나 추가해야 될 것이다.