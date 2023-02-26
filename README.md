## 필요할 때 마다 하나씩 정리해가는 라이브러리! 
## 중복이 될수도 있다!

### substring (int beginIndex) : 시작 인덱스부터 끝까지
### substring (int beginIndex, endIndex) : 시작 인덱스부터 끝 인덱스-1까지

```
String str = "0123456789";

str.substring(5); // 56789
str.substring(1,4); // 123 
```


### replace(), replaceAll(), replaceFirst()
### 문자열을 다른 문자열로 치환.
### 치환 메소드이긴 한데 주로 문자열에서 특정 문자를 삭제할때 유용하게 사용한다.

```
replace(CharSequence target, CharSequence replacement) : 모든 target replacement로 치환
String str = "a,b,c,d,e";
System.out.println(str.replace(",", " ")); // a b c d e
System.out.println(str.replace(",", "")); // abcde
replaceAll(String regex, String replacement) : replace()와 비슷하나, 첫번째 인자로 정규식을 넣는다.
```
```
replaceFirst(String target, String replacement) : 첫번째 발견되는 target만 치환한다.

String str = "a,b,c,d,e";
System.out.println(str.replaceFirst(",", " ")); // a b,c,d,e
System.out.println(str.replace(",", "")); // ab,c,d,e
```
