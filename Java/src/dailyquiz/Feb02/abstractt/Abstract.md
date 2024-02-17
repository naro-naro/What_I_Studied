# 추상 메소드
<p>자식클래스에서 반드시 오버라이드 해야만 사용할 수 있는 메소드</p>
<p>사기 클래스에서 반드시 추상메서드를 사용하도록하는 일종의 규제</p>

```
 abstract 리턴타입 메소드명() 
```

<br>

# 추상 클래스
<p>추상메소드를 하나 이상 갖는 클래스</p>

실체들의 공통 특성을 클래스로 빼놓은 것이
**추상클래스**

<p>추상클래스는 실체 클래스의 공통되는 필드와 메소드를 추출해 만들었기 때문에</p>
<p>객체를 직접 생성해 사용할 수 없다</p>
<p>new 연산자를 사용해 인스턴스를 생성할 수 없다</p>

**추상클래스는 실체 클래스를 만들기 위해 부모클래스로만 사용된다**

### 용도
- 실체 클래스들의 공통된 필드와 메소드의 이름을 통일
- 실체 클래스를 작성할 때의 시간 절약

### 선언
```
public abstract class 클래스명 {
	// 필드
	// 생성자
	// 메소드
}
```

### 추상클래스 오버라이딩
<p>추상클래스는 실체 클래스가 공통적으로 가져야 할 필드와 메소드를 정의해 놓은 추상적인 클래스이므로</p> 
<p>클래스의 멤버를 통일하는 게 목적</p>
<p>메소드의 선언만 통일하고</p>
<p>실행 내용은 클래스마다 달라야 하는 경우도 있다</p>
<p>abstract 메소드로 정의했음에도 실체(자식)클래스에서 해당 메소드를 구현하지 않는다면 컴파일 오류 발생</p>