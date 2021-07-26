---
title:  "[모각코] 1회차 결과"
excerpt: ""

categories:
  - 모각코
tags:
  - [Blog, jekyll, 모각코]

toc: true
toc_sticky: true

date: 2021-07-08
last_modified_at: 2021-07-08
---

### [최병욱](https://velog.io/@qowlz/%EB%AA%A8%EA%B0%81%EC%BD%94-1%ED%9A%8C%EC%B0%A8-%EA%B2%B0%EA%B3%BC)

![](https://media.vlpt.us/images/qowlz/post/2289931b-bff9-40e7-b70a-1d70a4d69903/%ED%99%94%EB%A9%B4%20%EC%BA%A1%EC%B2%98%202021-07-07%20192718.png)

목표로 설정한 1*, 1** class의 문제들을 2시간 30분 정도의 시간을 들여서 다 풀음.<br>
문제들이 너무 쉬워서 라이브러리를 사용하지않고 최대한 직접 구현하려고 노력했다.<br>
코딩을 처음 배우는 초보자들이 풀만한 문제들로만 구성되어있어서 c++의 기본에 대해 복습을 한 느낌이다.<br>
class 2에서는 조금 더 얻어가는 것이 많을것같다. 다음 회차를 기대해보려고 한다.

### [전규리](https://velog.io/@rlczl/2021-%ED%95%98%EA%B3%84-%EB%AA%A8%EA%B0%81%EC%BD%94-1%ED%9A%8C%EC%B0%A8-%EA%B2%B0%EA%B3%BC)
1차, 2차, 3차 목표 달성 후 [나비 모양 구현하기], [모래시계 모양 구현하기] 문제를 추가적으로 풀어보았다.
> **[1차 목표] 별찍기-5 피라미드 모양 구현하기**<br>
▼소스코드
```
import java.util.*;
public class star_2442 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int val = sc.nextInt();
		for (int i = 1; i <= val; i++) {
			for (int j = 0; j < val-i; j++) {
				System.out.print(" ");
			}
			for (int k = 0; k < 2 * i - 1; k++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
```
> **[2차 목표] 별찍기-6 역피라미드 모양 구현하기**<br>
▼소스코드
```
import java.util.*;
public class star_2443{
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int val = sc.nextInt();
		for (int i = 1; i <= val; i++) {
			for (int k = i; k > 1; k--) {
				System.out.print(" ");
			}
			for (int j = 0; j < 2*val-i-i+1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
```
> **[3차 목표] 별찍기-7 마름모 모양 구현하기**<br>
▼소스코드
```
import java.util.*;
public class star_2444 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int val = sc.nextInt();
		for (int i = 1; i <= val; i++) {
			for (int j = 0; j < val-i; j++) {
				System.out.print(" ");
			}
			for (int k = 0; k < 2 * i - 1; k++) {
				System.out.print("*");
			}
			System.out.println();
		}
		for (int i = 2; i <= val; i++) {
			for (int k = i; k > 1; k--) {
				System.out.print(" ");
			}
			for (int j = 0; j < 2 * val - i - i + 1; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
```
> **별찍기-8 나비 모양 구현하기**<br>
▼소스코드
```
import java.util.*;
public class star_2445 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int val = sc.nextInt();
		for (int i = 1; i <= val; i++) {
			for (int j = 0; j < i; j++) {
				System.out.print("*");
			}
			for (int j = 0; j < val*2-i*2; j++) {
				System.out.print(" ");
			}
			for (int j = i; j > 0; j--) {
				System.out.print("*");
			}
			System.out.println();
		}
		for (int i = val - 2; i >= 0; i--) {
			for (int j = i; j >= 0; j--) {
				System.out.print("*");
			}
			for (int j = val*2-i*2-2; j > 0 ; j--) {
				System.out.print(" ");
			}
			for (int j = 0; j <= i; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
```
> **별찍기-9 모래시계 모양 구현하기**<br>
▼소스코드
```
import java.util.*;
public class star_2446 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int val = sc.nextInt();
		for (int i = 0; i < val-1; i++) {
			for (int j = 0; j < i; j++) {
				System.out.print(" ");
			}
			for (int j = 0; j < 2*val-1-i-i; j++) {
				System.out.print("*");
			}
			System.out.println(" ");
		}
		for (int i = val-1; i >= 0; i--) {
			for (int j = 0; j < i; j++) {
				System.out.print(" ");
			}
			for (int j = 0; j < 2*val-1-i-i; j++) {
				System.out.print("*");
			}
			System.out.println();
		}
	}
}
```

### [문다연](https://velog.io/@dayo2n/%EC%96%B4%EC%BD%94%EB%AA%A8-2021-%ED%95%98%EA%B3%84-%EB%AA%A8%EA%B0%81%EC%BD%94-1%ED%9A%8C%EC%B0%A8-%EA%B2%B0%EA%B3%BC)
```
xcode의 오토레이아웃
	단말기 기종별로 레이아웃의 비율을 자동으로 맞춰주는 xcode의 시스템
    각각의 attribute는 constraints가 필요
class 연결하기 (drag)
	해당 스토리보드의 Custom Class에서 Class이름과 해당하는 swift파일의 이름을 맞춰야 함
	ctrl + drag 를 이용해 스토리보드에서 클래스와 연결
나머지 디테일은 코드 속 주석으로 처리

objects
- button : 버튼
- navigation controller : 화면 이동을 위한 오브젝트
- view controller (ui view) : 뷰
```

![](https://media.vlpt.us/images/dayo2n/post/e26e76c8-5d54-4fbe-bc4c-911c7a38f2f2/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202021-07-07%20%EC%98%A4%ED%9B%84%205.41.12.png)
< 오브젝트와 클래스를 연결하면 자동으로 함수가 생성되고, 생성된 함수에 입력한 명령대로 Move 버튼을 누르면 Click MOVE라고 콘솔에 출력되도록 한 결과 ><br>

![](https://media.vlpt.us/images/dayo2n/post/c0b9a776-2f82-4470-a172-dfac35194d40/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202021-07-07%20%EC%98%A4%ED%9B%84%206.04.56.png)

![](https://media.vlpt.us/images/dayo2n/post/9a82a763-9fa3-4a81-b674-f7c948fd5748/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202021-07-07%20%EC%98%A4%ED%9B%84%206.04.59.png)
< navigation contoller 오브젝트를 이용해 버튼을 클릭하면 화면을 위의 사진의 화면에서 아래 사진의 화면으로 이동하도록 한 결과 ><br>

### [장진영](https://velog.io/@zinzin22/2021-%ED%95%98%EA%B3%84-%EB%AA%A8%EA%B0%81%EC%BD%94-1%ED%9A%8C%EC%B0%A8-%EA%B2%B0%EA%B3%BC)
입출력과 사칙연산<br>
![](https://media.vlpt.us/images/zinzin22/post/5c4abf92-6a10-4f6b-96be-f19702357f74/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-07-07%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%208.50.51.png)

if문<br>
![](https://media.vlpt.us/images/zinzin22/post/c4d8babf-5831-41e8-a755-2d5cf6d6507a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202021-07-07%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%208.51.07.png)

> 결과
> - 입출력과 사칙연산 단계별 문제 모두 통과
> - if문 단계별 문제 모두 통과

> 느낀 점
> - 오랜만에 한 코딩이라 초반 부분에 실수가 많았다.
> - 아직은 초반 부분이라 문제들이 쉬웠던거 같다.
> - 조금은 늘은 실력에 자신감이 늘었다. 아주 조금..
> - 다음 단계 문제들이 기대가 된다.

### [한현준](https://damagedcode101.blogspot.com/2021/07/2021-1-77_7.html)
프로그램을 다 완성하지 못했습니다... ㅠ

> 소스코드(Java)

```
package codeTest;

import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc = new Scanner(System.in);
		String size = sc.nextLine();
		String[] size_list = size.split(" ");
		int N = Integer.parseInt(size_list[0]);
		int M = Integer.parseInt(size_list[1]);
		char[][] board = new char[N][M];


		int[] posB = new int[2];
		int[] posR = new int[2];
		int[] posO = new int[2];

		int COUNT = 0;

		for(int i = 0; i< N; i++) {
			String line = sc.nextLine();
			for(int j = 0; i<M; j++) {
				switch(line.charAt(j)) {
				case '#': board[i][j] = '#';
				break;
				case '.': board[i][j] = '.';
				break;
				case 'R': board[i][j] = 'R';
				break;
				case 'B': board[i][j] = 'B';
				break;
				case 'O': board[i][j] = 'O';
				break;
				default:break;
				}

				if(line.charAt(j) == 'B') {
					posB[0] = j;
					posB[1] = i;
				}
				if(line.charAt(j) == 'R') {
					posR[0] = j;
					posR[1] = i;
				}
				if(line.charAt(j) == 'O') {
					posO[0] = j;
					posO[1] = i;
				}
			}
		}
		sc.close();

		// move
//		while(COUNT < 10 && !(posR[0]==posO[0]&&posR[1]==posO[1]) && !(posB[0]==posO[0]&&posB[1]==posO[1])) {
//			COUNT++;
//
//			if(posR[0])
//
//		}

		// If Blue out: Fail.
		if (posB[0]==posO[0]&&posB[1]==posO[1]) {
			System.out.print(-1);
			return;
		}

		// If Count >= 10 and Red not out: Fail.
		if(COUNT >= 10 && !(posR[0]==posO[0]&&posR[1]==posO[1]){
			System.out.print(-1);
			return;
		}


	}

}
```

입력에 따라 보드를 2차원 배열에 저장하고 빨간 구슬, 파란 구슬, 구멍의 위치를 저장하였는데, 본격적으로 구슬들을 움직이는 알고리즘을 작성하는 부분에서 막혔습니다.
가령, 아래와 같은 예제의 경우,

```
5 5
#####
#..B#
#.#.#
#RO.#
#####
```
빨간구슬을 위로 움직이는 경우와 오른쪽으로 움직이는 경우 2가지가 있는데 둘을 모두 시도해야할 듯 한데 그것을 어떻게 구현할지 고민에 빠졌습니다. 결국에는 가능한 경우의 수를 전부 시도해야하는 것이 아닌가 합니다.
그래서 재귀 알고리즘을 사용해야 할 듯 한데...
더 연구가 필요한 상황입니다.

3시간에 한문제도 못 풀다니...! 삼성전자에 취직한다는 것은 역시 쉬운 일은 아니었습니다.
이 문제는 남는 시간에 틈틈이 풀도록 하고 다음 주 문제는 꼭 시간 안에 풀 수 있기를 기대해봅니다!

