# Text-mining
This is the repository of the project related to the text-mining using R programming languages.


## Regular Expression 정규 표현식
정규 표현식은 특정한 규칙을 가진 문자열을 표현하는 언어이다. 특정 조건에 해당하는 문자를 찾거나 수정할 때 정규 표현식을 사용한다. 
^: 시작하는것
$: 끝나는 것

택스트 안에서 $를 찾기 위해서는
\$($), ^\$ (맨앞 $), \$$(마지막 $)

.: 모든 character matching
......: 6 characters group matching
\.: character .
\..\. : character . + anycharacter + character .

[]: []안에 있는 모든 것들
[dH]. : d 또는 H 그리고 그 뒤에 아무 문자

[-]: range
[^]: 빼고 다

sub patter -> (a|b|c): a 또는 b 또는 c

Quantifiers *, +, ?: 
*: * 앞에 문자가 0개 이상
+: + 앞에 문자가 1개 이상
?: ? 앞에 문자가 없거나 1개

.*: 모든 텍스트
[-@]*: - 또는 @가 0개 이상

수량자 {}: {} 있는 숫자 만큼
.{5}: 어떤 character던지 5글자
[els]{1,3}: e l s 셋 중 1하나 이상 3개 이하
[a-z]{3,}: 3개이상의 단어
.*?: 수량자 최소 단위 0으로 바뀜

정규표현식 사이트 = [regexr](gskinner.com/RegExr/)


(reference: Do it! R text mining)
