# 👊묵찌빠 게임 프로젝트


## 목차
- [소개](#소개)
- [프로젝트 수행 중 핵심 경험](#프로젝트-수행-중-핵심-경험)
- [타임라인](#타임라인)
- [파일구조](#파일구조)
- [순서도](#순서도)
- [실행화면](#실행화면)
- [팀 규칙](#팀-규칙)
- [트러블 슈팅](#트러블-슈팅)
- [7팀 회고](#7팀-회고)

## 🗣소개
### 프로젝트 소개
#### 프로젝트 기간 : 22.12.26 ~ 22.12.30
- 가위바위보를 승자가 날 때까지 반복한다.(0 누르면 종료)
- 가위바위보 승자가 턴을 잡고 묵찌빠 게임을 한다.(0 누르면 종료)
- 턴을 잡고 있을때 같은 모양을 내면 묵찌빠 게임을 승리한다.
- 같은 모양이 나오지 않으면 게임을 반복한다. (0 누르면 종료)

### 팀 소개
- 팀 구성원(2인)

| vetto | 송준 |
| :--------: | :--------: |
| <img src="https://cdn.discordapp.com/attachments/535779947118329866/1055718870951940146/1671110054020-0.jpg" width="300" height="350"/> | <img src="https://user-images.githubusercontent.com/88870642/210026753-591175fe-27c1-4335-a2cb-f883bfeb2784.png" width="300" height="300"/>|
|Navigator, Driver|Navigator, Driver|


## 📍프로젝트 수행 중 핵심 경험
<details>
    <summary><big>핵심 경험</big></summary>
- Swift의 Optional 안전하게 처리하기<br>
- if와 switch 조건문의 차이와 장단점 비교해보기<br>
- 순환함수(재귀함수)와 반복문의 장단점 비교해보기<br>
- 함수가 한 가지 일만 하도록 기능 분리하기<br>
- guard 구문의 이해와 활용<br>
- Git의 커밋단위 고민하고 커밋에 적용하기<br>
- Git 커밋 로그 형식에 맞춰 커밋하기<br>
- 코딩 컨벤션 고민하기<br>
- 동료와 협업자세 고민하기<br>
</details>


## ⏱타임라인
#### STEP 1 [2022.12.26~2022.12.27]
- **2022.12.26**
    - 숫자 입력 함수 구현, 컴퓨터 숫자 반환 함수 구현
    - 숫자를 가위바위보로 바꾸는 함수 구현
    - 비교하여 결과 반환 함수 구현
- **2022.12.27**
    - 가위바위보 메뉴 출력 함수 구현
    - 비교하는 함수 Naming 변경 및 refactoring
    - 가위바위보 결과 출력함수 구현

#### STEP 2 [2022.12.28~2022.12.30]
- **2022.12.28**
    - 승자 타입 분리
    - 입력 에러처리로 구현
    - 턴과 묵찌빠 메뉴 출력 함수 구현
    - 숫자를 묵찌빠로 바꾸는 함수 구현
    - 묵찌빠 결과 반환 함수 구현
- **2022.12.29**
    - 묵찌빠 결과 반환 함수 refactoring
    - 가위바위보 함수 refactoring
    - runGame함수 구현
    - 묵찌빠 결과 출력함수 구현

## 📂파일구조
```bash!
RockPaperScissors
├── Error.swift
├── MookZziBbaGame.swift
├── ReturnNumberLibrary.swift
├── RockPaperScissorsGame.swift
├── StartGame.swift
├── Type
│   ├── MookZziBbaType.swift
│   ├── RockPaperScissorsType.swift
│   └── WinnerType.swift
└── main.swift
```

## 순서도

<details>
<summary><big>STEP 1 순서도</big></summary>
<img src="https://cdn.discordapp.com/attachments/1056776760622071858/1058265379266363402/RockPaperScissorsGame.drawio.png"/>
</details>

<details>
<summary><big>STEP 2 순서도</big></summary>
<img src="https://cdn.discordapp.com/attachments/1056776760622071858/1058266474327855145/MookZziBbaGame.drawio.png"/>
</details>

## 💻실행화면
|**게임 실행**|
|---|
|![컴퓨터승리](https://user-images.githubusercontent.com/88870642/210028600-7db422a6-2f80-4ed3-9d25-7515aec3a589.gif)|
|**게임 종료**|
|![게임종료](https://user-images.githubusercontent.com/88870642/210028798-19f927b4-6857-454d-886f-c5893fe22612.gif)|
|**입력 오류**|
|![잘못된 입력](https://user-images.githubusercontent.com/88870642/210028731-ad50bc47-de29-4815-a288-396d9b9ea202.gif)|
|**묵찌빠 입력오류 시 턴 넘김**|
|![묵찌빠잘못입력](https://user-images.githubusercontent.com/88870642/210028821-3f210ce5-8b6c-489c-8c95-b5847a732072.gif)|


## 👥팀 규칙
### 코드 컨벤션
- 함수 선언 시 100자 이상으로 넘어갈 경우 매개변수 줄바꾸기
- 함수, 변수, 상수 이름은 CamelCase 사용하기
- 변수명 모호하게 작성하지 않기
- 부호, 등호 양쪽으로 띄어써주기
- 맥락상 의미가 달라지면 줄바꾸기

### 커밋 컨벤션
- feat : 기능 추가 (새로운 기능)
- refactor : 리팩토링 (네이밍 수정 등)
- docs : 문서 변경 (문서 추가, 수정, 삭제)
- chore : 기타 변경사항 (코드의 변화가 생산적인 것이 아닌 것 수정)


## 🔥트러블 슈팅
### 1️⃣ Naming
프로젝트를 진행함에 있어 Naming이 정말 까다로웠습니다. 그 중 가장 큰 이유는 사용자 타입을 사용하지 않아서 그랬던거 같습니다. 예를 들어 class 타입으로 "RockPaperScissors"로 설정을 해주었다면, 여러 기능을 하는 함수의 함수명에서 "RockPaperScissors"를 작성하지 않아도 될 것입니다.

**- class 사용**
```swift=
class RockPaperScissors {
    func decideWinner() {
        // 승리자를 결정 지음        
    }
    func printWinner() {
        // 승리자를 프린트함
    }
}
```

**- class 미사용**
```swift=
func decideRockPaperScissorsGameWinner() {
    
}

func printRockPaperScissorsGameWinner() {
    
}
```
클래스 타입의 용도와 기능은 다양하지만, 클래스와 관련된 함수를 묶어줌으로써 함수의 Naming을 단축시킬 수 있다고 생각됩니다.

------
### 2️⃣ 가위바위보 로직 구현
가위바위보 로직 구현에 있어서 사용자의 숫자와 컴퓨터의 숫자를 빼서 승패를 결정짓는 로직을 생각했습니다. 하지만 나중에 가위바위보를 결정 짓는 숫자들이 변경된다면 프로그램에서 전체적인 리팩토링이 필요할 것입니다. 이러한 이유로 숫자가 아닌 가위,바위,보로 승패를 확인할 수 있는 로직을 구현했습니다. 이 과정 중 enum을 통해 제한적인 조건으로 가위, 바위, 보를 선언해주었습니다.

**- 수정 전(숫자로 로직처리)**
숫자값의 뺄셈을 통해 로직을 구현했지만, 숫자가 변경될 시 리팩토링이 필요합니다.
```swift=
func compareHand(computerHand: Int, userHand: Int) -> String {
    let status: String

    if result == 0 {
        status = "Draw"
    } else if result == -2 || result == 1 {
        status = "Win"
    } else {
        status = "Lose"
    }

    return status
}
```

**- 수정 후(가위, 바위, 보로 로직처리)**
열거체형태로 숫자가 변경되도 가위, 바위, 보가 선언된 열거체에서만 변경하면 됩니다.
```swift=
func decideRockPaperScissorWinner(_ userHand: RockPaperScissors,
                                  _ computerHand: RockPaperScissors) -> Winner {
    switch (userHand, computerHand) {
    case (.scissors, .paper), (.rock, .scissors), (.paper, .rock):
        return .user
    case (.scissors, .rock), (.rock, .paper), (.paper, .scissors):
        return .computer
    default:
        return .draw
    }
}
```

**- Enum 타입**

```swift=
enum RockPaperScissors: Int {
    case scissors = 1
    case rock = 2
    case paper = 3
    case wrongHand
}
```
---

### 3️⃣ 에러처리
처음 코드를 작성할 때 에러처리를 따로 두지 않고 작성했습니다. 그 이유는 step1에서는 에러처리를 안해도 구현을 할 수 있었기 때문입니다. 그러나  step2를 시작하고 보니 에러처리를 이용해서 구현해야 project에서 요구하는 사항들이 정상적으로 작동된다는 것을 알게되었습니다. 그 결과 코드안에 에러처리를 포함하게 리팩토링하였고 저희가 원하던 기능분리에도 성공하게 되었습니다.


---

### 4️⃣ 기능분리
- 함수가 하나의 기능을 가지도록 분리시키려고 노력했습니다. 그 이유는 재사용 측면입니다. 여러 기능을 가지고 있는 함수 중 한개의 기능만 재사용해야 할 때, 재사용하지 못하고 새로운 함수를 만들어야 하는 불편함이 있기 때문입니다.
- makeRandomComputerNumber(), func inputUserNumber()가 기능분리가 잘된 케이스입니다.

---

### 5️⃣ enum
 enum타입을 통해 값을 불러올 때 "**rawValue**"를 사용했습니다. .rawValue"는 호출될때 불명확한 이름으로 의미를 파악하기가 어렵습니다. 이를 해결하기 위해 enum타입에서 연산 프로퍼티를 사용해서 처리했습니다. 연산 프로퍼티를 통해 ".rawValue"가 아닌 "name"이라고 지정하여 모호함을 벗어났습니다.


**- 변경 전**
```swift=
enum winner: String {
    case user = "사용자"
    case computer = "컴퓨터"
    case draw 
}
```

**- 변경 후**
```swift=
enum Winner {
    case user
    case computer
    case draw
    
    var name: String {
        switch self {
        case .user:
            return "사용자"
        case .computer:
            return "컴퓨터"
        case .draw:
            return "무승부"
        }
    }
}
```
**- 호출시**
```swift=
print(Winner.rawValue) //변경 전

print(Winner.name) //변경 후
```


---

### 6️⃣ 함수의 재사용성 

- 묵찌빠게임과 가위바위보게임에서 재사용할 수 있다고 판단된 "**inputUserNumber**"함수를 리팩토링했습니다.
- 수정전에는 "**printMenu()**"(가위바위보로직에 사용되는 함수)가 있어서 묵찌빠 게임에 재사용할 수 없었지만, "**printMenu()**"삭제, 간단한 로직 변경 등의 리팩토링을 거쳐 재사용 가능한 함수로 만들었습니다.

**- 수정 전**
```swift=
func inputUserNumber() -> Int {
    printMenu()
    guard let userInput = readLine() else {
        return inputUserNumber()
    }
    guard let userNumber = Int(userInput) else {
        print("잘못된 입력입니다. 다시 시도해주세요.")
        return inputUserNumber()
    }
    return userNumber
}
```

**- 수정 후**
```swift=
func inputUserNumber() throws -> Int {
    guard let userInput = readLine(), let userNumber = Int(userInput) else {
        throw InputError.invalidInput
    }
    return userNumber
}
```

## 7팀 회고
* [7팀 회고](https://github.com/gzzjk159/ios-rock-paper-scissors/blob/step2/7%ED%8C%80%20%ED%9A%8C%EA%B3%A0.md)
