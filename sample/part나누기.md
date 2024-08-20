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




### 코드 비교 가능한것
---

<table>
  <tr>
    <th>코드 1</th>
    <th>코드 2</th>
  </tr>
  <tr>
    <td>
      <pre><code>
// JavaScript 예시
function hello() {
  console.log("Hello, World!");
}
      </code></pre>
    </td>
    <td>
      <pre><code>
# Python 예시
def hello():
    print("Hello, World!")
      </code></pre>
    </td>
  </tr>
</table>


만약 HTML을 사용하지 않고 Markdown만 사용하려면, 코드 블록(```)을 테이블 내에서 직접 사용할 수 없습니다. 하지만 **백틱(`)**을 사용해 인라인 코드를 표시할 수 있습니다.
| 코드 1 | 코드 2 |
| ------ | ------ |
| `function hello() { console.log("Hello, World!"); }` | `def hello(): print("Hello, World!")` |


GitHub Markdown에서 테이블 안에 코드 블록을 삽입할 때, 마크다운 구문(```) 자체가 렌더링되지 않는 문제를 해결하는 방법은 아래와 같이 "코드 블록을 이스케이프(escape)"하는 것입니다. 이를 통해 코드 블록이 테이블 안에 올바르게 표시되도록 할 수 있습니다.

GitHub에서는 코드 블록을 테이블 안에 넣으려면 인라인 코드(``` ``) 형식으로 처리하는 것이 아니라 HTML 코드 블록을 사용하는 방법이 더 적합합니다.

HTML을 활용한 테이블 내 코드 블록 예시
HTML 태그를 사용하여 테이블 안에 코드를 삽입하면 ``` 표식이 제대로 나타나지 않게 됩니다.
