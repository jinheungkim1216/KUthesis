# KU Thesis

건국대 졸업논문 $\LaTeX$ 스타일 양식.

2024년 후기 기준으로 [상허기념도서관-학위논문](https://library.konkuk.ac.kr/research/thesis-guide), [건국대 디콜렉선](https://konkuk.dcollection.net)을 참고해서 제작되었습니다.

파일 구성은 다음과 같습니다.
- `KUthesis.sty`: 스타일 양식
- `example_eng.tex`: 영문 예제 파일
- `example_kor.tex`: 국문 예제 파일
- `example.bib`: 예제 bib 파일

---

## 예시
```
\documentclass[11pt]{report}
\usepackage{KUthesis} % 기본 lang=eng, type=doctor
%\usepackage[lang=eng, type=doctor]{KUthesis}
% lang = eng, kor
% type = doctor, master

\begin{document}
<setting>
<main text>
\end{document}
```

---
## 논문 설정

### 기본정보
**논문 제목**
- `\thesisTitle`: 논문 영어 제목
- `\thesisSubTitle`: 논문 영어 부제목
- `\thesisTitleKO` : 한글 논문 제목
- `\thesisSubTitleKO`: 한글 논문 부제목

부제목이 없을시에는 `\thesisSubTitle{}`, `\thesisSubTitleKO{}`로 처리.

**논문 정보**
- `\thesisDateFront`: 학위 수여일 (전기 2월, 후기 8월)
- `\thesisDateSubFront`: 청구 년월 (전기 10,11월, 후기 4,5월)
- `\thesisDateApproval`: 최종심사 년월 (전기 11,12월, 후기 5,6월) 
- `\thesisSupervisor`: 지도교수 이름
- `\thesisDegree`: 학위 (석사: Master of Science in Physics, 박사: Doctor of Philosophy in Physics, 대학원홈페이지 참고)
- 
**저자 정보**
- `\thesisLastName` : 이름
- `\thesisFirstName` : 성
- `\thesisDepartment`: 학과
- `\thesisSchool` : 대학원 이름 (일반대학원)

- `\thesisLastNameKO` : 한글 이름
- `\thesisFirstNameKO` : 한글 성
- `\thesisDepartmentKO` : 한글 학과이름
- `\thesisSchoolKO` : 한글 대학원 이름

**심사위원**
- `\thesisCommitteeI`
- `\thesisCommitteeII`
- `\thesisCommitteeIII`
- `\thesisCommitteeIV`
- `\thesisCommitteeV`
빈 인준지가 필요할시 `\thesisCommittee{}`로 처리.

**초록 키워드**
- `\thesisKeywords` : 영문 키워드
- `\thesisKeywordsKor`: 한글 키워드

### 페이지
- `\makeKUfront`: 논문 표지
- `\makeKUsubfront`: 논문 속지
- `\makeKUapproval`: 인준지
- `\begin{KUabstract} <text> \end{KUabstract}` : 영문 초록
- `\begin{KUabstractKO} <text> \end{KUabstractKO}` : 한글 초록

영문논문일시 영문초록을 본문 앞에, 국문초록을 논문 마지막에 작성하며, 국문논문일시 국문초록을 본문 앞에, 영문초록을 논문 마지막에 작성합니다.

---
## 기타

양식 변경, 버그, 오타, 문의사항 또는 기능추가가 필요한 경우 편하게 jinheung.kim1216@gmail.com 으로 연락주시기 바랍니다.

국문논문 양식 작성은 [김현수](https://github.com/hyeonsoo-kim)님꼐서 기여해주셨습니다.