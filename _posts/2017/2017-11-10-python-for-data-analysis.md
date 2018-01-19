## 윈도우용 설치와 설정

### Anaconda 설치

* Anaconda를 설치한다
* 주요 과학계산 파이썬 커뮤니티는 아직 파이썬 3으로 넘어가지 않았으므로 파이썬 2.7 버전을 권장
* 다운로드 링크: [https://repo.continuum.io/archive/Anaconda2-5.0.1-Windows-x86\_64.exe](https://repo.continuum.io/archive/Anaconda2-5.0.1-Windows-x86_64.exe)

### 파이썬 정상 설치 확인

* 시작 메뉴에서 명령행\(cmd.exe\)을 열고 python이라고 입력해서 파이썬 인터프리터를 실행하자.
* 그러면 터미널에 방금 설치한 아나콘다의 버전 정보가 포함된 메시지가 출력된다.
* 아나콘다의 버전 정보가 다르거나 잘 동작하지 않는다면 윈도우 환경변수를 살펴보자.

Anaconda 정상 설치 확인

* 설치를 마친 후에 명령행 프롬프트를 열어서 다음 명령을 실행시켜보자.

```
jupyter notebook
```

* Jupyter를 실행시키고 pandas를 import하여 간단한 matpltlib 그래프를 만들어서 정상적으로 설치됐는지 확인해보자.

### 통합 개발 환경

* 기본 개발 환경은 'Jupyter와 텍스트 편집기'이다. Jupyter에서 각 코드 조각을 테스트하고 디버깅한다.
* 이 방법은 데이터를 쌍방향으로 다룰 수 있으며, 특정한 데이터 묶음에 대한 조작이 제대로 되고 있는지 시각적으로 확인이 가능해서 상당히 유용하다.
* 텍스트 편집기 대시 IDE를 선호할 경우에는 파이참\(Pycharm\)을 이용하면 된다.

### 데이터 파일과 관련 자료

* Github 저장소에서 구하면 된다.
* [http://github.com/pydata/pydata-book](http://github.com/pydata/pydata-book)



