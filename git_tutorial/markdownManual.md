# 마크다운 사용법 정리
## 마크다운 문법
### 1. 헤더
- 문서 제목 (큰 제목)

   ```
   This is Markdown Title H1 1
   ========================
   ```

   ```
   # This is Markdown Title H1 2
   ```
  
  + 적용 예시
  
    This is Markdown Title H1 1
    ========================
  
    # This is Markdown Title H1 2
  
- 문서 부제목 (작은 제목)
 
  ```
  This is Markdown Subtitle H2 1
  ---------------------------
  ```
 
  ```
  ## This is Markdown Subtitle H2 2
  ```

  + 적용 예시
  
    This is Markdown Subtitle H2 1
    ---------------------------

    ## This is Markdown Subtitle H2 2

- 기타 글머리 형식
 
  ```
  ### This is a H3
  #### This is a H4
  ##### This is a H5
  ###### This is a H6
  ```
 
  + 적용 예시
  
    ### This is a H3
    #### This is a H4
    ##### This is a H5
    ###### This is a H6
    ####### This is a H7 (H6까지만 지원)

### 2. 인용구 (BlockQuote)
- ```>``` 사용

  ```
  > This is a first quote
  > > This is a second quote
  > > > This is a third quote
  ```
  
  + 적용 예시
  
    > This is a first quote
    > > This is a second quote
    > > > This is a third quote


### 3. 목록
- 순서있는 목록은 숫자와 점을 같이 사용

  ```
  1. ㄱㄴㄷ
  2. ㄹㅁㅂ
  3. ㅅㅇㅈ
  ```

  + 적용 예시
  
    1. ㄱㄴㄷ
    2. ㄹㅁㅂ
    3. ㅅㅇㅈ

- 숫자의 순서는 무조건 내림차순으로 정렬

  ```
  1. ㄱㄴㄷ
  3. ㅅㅇㅈ
  2. ㄹㅁㅂ
  ```
  
  + 적용 예시
  
    1. ㄱㄴㄷ
    3. ㅅㅇㅈ
    2. ㄹㅁㅂ

- 순서없는 목록의 경우 ```*```, ```+```, ```-``` 중 무작위 사용 (혼합 사용 가능)
  
  ```
  * ㄱ
    * ㄴ
      * ㄷ
  
  + ㄱ
    + ㄴ
      + ㄷ
  
  - ㄱ
    - ㄴ
      - ㄷ
  ```

  + 적용 예시
  
    * ㄱ
      * ㄴ
        * ㄷ
    
    + ㄱ
      + ㄴ
        + ㄷ
    
    - ㄱ
      - ㄴ
        - ㄷ

### 4. 코드
- 들여쓰기 방식 : 4개의 공백(스페이스바) 또는 1개의 탭으로 들여쓰기를 할 경우 들여쓰지 않은 행까지 코드 블록으로 변환

  ```
  This is a normal sentence.
  
      This is a code sentence.
   
  This is a normal sentence.
  ```
  
  + 적용 예시
  
    This is a normal sentence.
        
        This is a code sentence.
    
    This is a normal sentence.
    
- 코드 블록을 사용할 행 위 아래로 한 줄 띄어쓰지 않으면 인식이 안되는 문제 발생

  ```
  This is a normal sentence.
      This is a code sentence.
  This is a normal sentence.
  ```
  
  + 적용 예시
    
    This is a normal sentence.
        This is a code sentence.
    This is a normal sentence.

 - ```<pre><code>코드</code></pre>``` 방식
 
   ```
   <pre>
   <code>
   코드
   </code>
   </pre>
   ```
   
   + 적용 예시
   
     <pre>
     <code>
     코드
     </code>
     </pre>

 - ``` ` ``` 방식
 
   <pre>
   <code>
   ```
   코드
   ```
   </code>
   </pre>
   
   + 적용 예시
     
     ```
     코드
     ```
     
### 5. 수평선
- 보통 페이지 나누기 용도로 사용

  ```
  * * *
  
  ***
  
  *****
  
  - - -
  
  -----------------------------
  ```
  
  + 적용 예시
  
    * * *
    
    ***
    
    *****
    
    - - - 
    
    --------------------------------
    
### 6. 링크
 - 참조 링크
 
   ```
   Link : [Google][https://google.com "Go google"]
   ```
   
   + 적용 예시
   
     Link : [Google][https://google.com "Go google"]
 
 - 외부 링크
 
   ```
   Link : [Google](https://google.com, "Go google")
   ```
   
   + 적용 예시
   
     Link : [Google](https://google.com, "Go google")
     
 - 자동 연결
   
   ```
   외부링크 : <https://google.com/>
   이메일링크 : <email@email.com>
   ```
   
   + 적용 예시
   
     외부링크 : <https://google.com/>
     이메일링크 : <email@email.com>
     
### 7. 강조

   ```
   *ABCDEFG*
   _ABCDEFG_
   **ABCDEFG**
   __ABCDEFG__
   ~~ABCDEFG~~
   ```
   
   + 적용 예시
   
     *ABCDEFG*
     _ABCDEFG_
     **ABCDEFG**
     __ABCDEFG__
     ~~ABCDEFG~~

### 8. 이미지

   ```
   ![Alt text](/path/to/img.jpg)
   ![Alt text](/path/toimg.jpg "Optioanl Title")
   ```
   
 - 사이즈 조절은 ```<img width="" heiht=""></img>``` 이용
 
   ```
   <img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
   <img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
   ```
   
### 9. 줄바꿈
 - 3칸 이상 공백(스페이스바)(```   ```) 입력
 
   ```
   * 줄 바꿈을 하기 위해 문장 마지막에서 3칸 이상 띄어쓰기 실행,
   이렇게
   
   * 줄 바꿈을 하기 위해 문장 마지막에서 3칸 이상 띄어쓰기 실행,   
   이렇게
   ```
   
   + 적용 예시
     
     * 줄 바꿈을 하기 위해 문장 마지막에서 3칸 이상 띄어쓰기 실행,
     이렇게
     
     * 줄 바꿈을 하기 위해 문장 마지막에서 3칸 이상 띄어쓰기 실행,   
     이렇게
