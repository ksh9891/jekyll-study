# 소개
jekyll 을 배워서 블로그 커스터마이징 하고싶다.

# 목표
- jekyll 습득 후 hydejack 테마 기반으로 만들어진 블로그 커스터 마이징!!!!

# Jekyll ?
Jekyll 은 아주 심플하고 블로그 지향적인 "정적 사이트 생성기".  
텍스트(마크다운) 파일로 컨텐츠를 작성하고, 폴더로 그 파일들을 정리합니다. 다음, Liquid 기능이 추가된 HTML 템플릿을 사용해 사이트의 모양을 만듭니다. Jekyll 은 자동으로 내용물과 템플릿들을 함께 합쳐서, 어떤 서버에서도 올바르게 작동하는, 완전한 정적 웹사이트를 생성합니다.

# Jekyll 사이트 구조
## 구조
모두 다 그런건 아니고, 일반적인 구조
```terminal
.
├── _config.yml
├── _data
|   └── members.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.md
|   └── on-simplicity-in-technology.md
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.md
|   └── 2009-04-26-barcamp-boston-4-roundup.md
├── _sass
|   ├── _base.scss
|   └── _layout.scss
├── _site
├── .jekyll-metadata
└── index.html # 'index.md' 이어도 되지만 올바른 YAML 머리말이 필요합니다
```

## 하는 일
| File / Directory  | Description                                                                                       |
| :-------------:   | :------------------------------------------------------------------------------------------------ |
| _config.yml       | 환경설정 정보                                                                                     |
| _drafts           | 아직 게시하지 않은 포스트 저장소                                                                  |
| _includes         | 재사용하기 위한 파일을 담는 곳                                                                    |
| _layouts          | 포스트를 포장할 때 사용하는 템플릿                                                                |
| _posts            | 내 컨텐츠 저장소,<br>반드시 다음과 같은 명명 규칙을 사용해야 한다.<br>YEAR-MONTH-DAY-title.MARKUP |
| _data             | 사이트에 사용할 데이터를 적절한 포맷으로 정리하여 보관하는 디렉토리                               |
| _sass             | Sass 조각파일 저장                                                                                |
| _site             | Jekyll 이 변환 작업을 마친 뒤 생성된 사이트가 저장되는 (디폴트) 경로                              |
| .jekyll-metadata  | Jekyll 은 이 파일을 참고하여, 마지막으로 빌드한 이후에 한번도 수정되지 않은 파일은 어떤 것인지, 다음 빌드 때 어떤 파일을 다시 생성해야 하는지 판단할 수 있다. |