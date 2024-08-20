# 단락 나누기

## 단락 Notion처럼 분리해서 표시하는 방법

### 문단 단락 나누기

- 1
- 2
- 3
- 4


### 단락나누기

<div style="display: flex;">
  <div style="flex: 1; padding-right: 10px;">
    ### 왼쪽 내용
    여기에 왼쪽에 표시할 내용을 작성합니다.
    - 작성자
    - 내용
    
  </div>
  
  <div style="flex: 1; padding-left: 10px;">
    ### 오른쪽 내용
    여기에 오른쪽에 표시할 내용을 작성합니다.
    - 작성자 
    - 내용
    
  </div>
</div>

### 단락나누기2
| 왼쪽 내용 | 오른쪽 내용 |
| --------- | ----------- |
| 여기에 왼쪽에 표시할 내용을 작성합니다. | 여기에 오른쪽에 표시할 내용을 작성합니다. |
| 작성자 코드 | 작성자 코드 |
| ```code ``` | ```code ``` |


<div>
<table style="border:none; width: 100%;">
  <tr>
    <td style="border:none; width: 50%;">
      왼쪽 내용
      - A
      - B
      - C
    </td>
    <td style="border:none; width: 50%;">
      ### 오른쪽 내용
      1. AAA
      2. dddd
      3. 44444
    </td>
  </tr>
</table>
</div>


### 코드 비교 및 분류

| 코드 1 | 코드 2 |
| ------ | ------ |
| ```js                           | ```python                  |
| function hello() {              | def hello():               |
|   console.log("Hello, World!"); |     print("Hello, World!") |
| }                               | ```                        |
| ```                             |                            |

