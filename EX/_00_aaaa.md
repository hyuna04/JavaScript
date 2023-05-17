# 출력문
dom: 문서객체모델
json: Javascript 객체 리터럴 문법을 따르는 문자열
JSON 안에는 Javascript의 기본 데이터 타입인 문자열, 숫자, 배열, 불리언 그리고 다른 객체를 포함할 수 있음


## window.alert() 메소드
- 자바스크립트에서 가장 간단하게 데이터를 출력할 수 있는 방법은 window.alert() 메소드를 이용하는 것
- <script>
    function alertDialogBox() {
        alert("~~");
    }
</script>

## HTML DOM 요소를 이용한 innerHTML 프로퍼티
- 실제 자바스크립트 코드에서 출력을 위해 가장 많이 사용되는 방법은 HTML DOM 요소를 이용한 innerHTML 프로퍼티를 이용하는 방법
- 우선 document 객체의 getElementByID()나 getElementsByTagName() 등의 메소드를 사용하여 HTML 요소를 선택한 후 innerHTML 프로퍼티를 이용하면 선택된 HTML 요소의 내용(content)이나 속성(attribute)값 등을 손쉽게 변경할 수 있음
- <script>
    var str = document.getElementById("text");
    str.innerHTML = "이 문장으로 바뀌었습니다!";
</script>

## document.write() 메소드
- document.write() 메소드는 웹 페이지가 로딩될 때 실행되면, 웹 페이지에 가장 먼저 데이터를 출력
- 하지만 웹 페이지의 모든 내용이 로딩된 후에 document.write() 메소드가 실행되면, 웹 페이지 내에 먼저 로딩된 모든 데이터를 지우고 자신의 데이터를 출력하게 됨

## console.log() 메소드
- console.log() 메소드는 웹 브라우저의 콘솔을 통해 데이터를 출력해 줌

# 변수선언
ES6 이전에서는 var 키워드 사용하여 변수선언
ES6 이후 let, const 키워드 사용하여 변수선언