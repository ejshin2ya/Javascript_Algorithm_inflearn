## 7-1. 선택정렬

N개의 숫자가 입력되면 오름차순으로 정렬하여 출력하는 프로그램을 작성하세요.
정렬하는 방법은 선택정렬입니다.
▣ 입력설명
첫 번째 줄에 자연수 N(1<=N<=100)이 주어집니다.
두 번째 줄에 N개의 자연수가 공백을 사이에 두고 입력됩니다. 각 자연수는 정수형 범위 안에
있습니다.
▣ 출력설명
오름차순으로 정렬된 수열을 출력합니다.
▣ 입력예제 1
6
13 5 11 7 23 15
▣ 출력예제 1
5 7 11 13 15 23

## 7-2. 버블정렬

N개의 숫자가 입력되면 오름차순으로 정렬하여 출력하는 프로그램을 작성하세요.
정렬하는 방법은 버블정렬입니다.
▣ 입력설명
첫 번째 줄에 자연수 N(1<=N<=100)이 주어집니다.
두 번째 줄에 N개의 자연수가 공백을 사이에 두고 입력됩니다. 각 자연수는 정수형 범위 안에
있습니다.
▣ 출력설명
오름차순으로 정렬된 수열을 출력합니다.
▣ 입력예제 1
6
13 5 11 7 23 15
▣ 출력예제 1
5 7 11 13 15 23

## 7-3. special Sort(구글 인터뷰)

N개의 정수가 입력되면 당신은 입력된 값을 정렬해야 한다.
음의 정수는 앞쪽에 양의정수는 뒷쪽에 있어야 한다. 또한 양의정수와 음의정수의 순서에는
변함이 없어야 한다.
▣ 입력설명
첫 번째 줄에 정수 N(5<=N<=100)이 주어지고, 그 다음 줄부터 음수를 포함한 정수가 주어진
다. 숫자 0은 입력되지 않는다.
▣ 출력설명
정렬된 결과를 출력한다.
▣ 입력예제 1
8
1 2 3 -3 -2 5 6 -6
▣ 출력예제 1
-3 -2 -6 1 2 3 5 6

## 7-4. 삽입정렬

N개의 숫자가 입력되면 오름차순으로 정렬하여 출력하는 프로그램을 작성하세요.
정렬하는 방법은 삽입정렬입니다.
▣ 입력설명
첫 번째 줄에 자연수 N(1<=N<=100)이 주어집니다.
두 번째 줄에 N개의 자연수가 공백을 사이에 두고 입력됩니다. 각 자연수는 정수형 범위 안에
있습니다.
▣ 출력설명
오름차순으로 정렬된 수열을 출력합니다.
▣ 입력예제 1
6
11 7 5 6 10 9
▣ 출력예제 1
5 6 7 9 10 11

## 7-5. Least Recently Used(카카오 캐시 문제 변형)

캐시메모리는 CPU와 주기억장치(DRAM) 사이의 고속의 임시 메모리로서 CPU가 처리할 작업
을 저장해 놓았다가 필요할 바로 사용해서 처리속도를 높이는 장치이다. 워낙 비싸고 용량이
작아 효율적으로 사용해야 한다. 철수의 컴퓨터는 캐시메모리 사용 규칙이 LRU 알고리즘을 따
른다. LRU 알고리즘은 Least Recently Used 의 약자로 직역하자면 가장 최근에 사용되지 않
은 것 정도의 의미를 가지고 있습니다. 캐시에서 작업을 제거할 때 가장 오랫동안 사용하지
않은 것을 제거하겠다는 알고리즘입니다.
만약 캐시의 사이즈가 5이고 작업이
2 3 1 6 7 순으로 저장되어 있다면,
(맨 앞이 가장 최근에 쓰인 작업이고, 맨 뒤는 가장 오랫동안 쓰이지 않은 작업이다.)

1. Cache Miss : 해야할 작업이 캐시에 없는 상태로 위 상태에서 만약 새로운 작업인 5번 작
   업을 CPU가 사용한다면 Cache miss가 되고 모든 작업이 뒤로 밀리고 5번작업은 캐시의 맨
   앞에 위치한다.
   5 2 3 1 6
   (7번 작업은 캐시에서 삭제된다.)
2. Cache Hit : 해야할 작업이 캐시에 있는 상태로 위 상태에서 만약 3번 작업을 CPU가 사용
   한다면 Cache Hit가 되고, 63번 앞에 있는 5, 2번 작업은 한 칸 뒤로 밀리고, 3번이 맨 앞으
   로 위치하게 된다.
   5 2 3 1 6
   --->
   3 5 2 1 6
   캐시의 크기가 주어지고, 캐시가 비어있는 상태에서 N개의 작업을 CPU가 차례로 처리한다면
   N개의 작업을 처리한 후 캐시메모리의 상태를 가장 최근 사용된 작업부터 차례대로 출력하는
   프로그램을 작성하세요.
   ▣ 입력설명
   첫 번째 줄에 캐시의 크기인 S(3<=S<=10)와 작업의 개수 N(5<=N<=1,000)이 입력된다.
   두 번째 줄에 N개의 작업번호가 처리순으로 주어진다. 작업번호는 1 ~100 이다.
   ▣ 출력설명
   마지막 작업 후 캐시메모리의 상태를 가장 최근 사용된 작업부터 차례로 출력합니다.
   ▣ 입력예제 1
   5 9
   1 2 3 2 6 2 3 5 7
   ▣ 출력예제 1
   7 5 3 2 6

## 7-6.장난꾸러기 현수

새 학기가 시작되었습니다. 현수는 새 짝꿍을 만나 너무 신이 났습니다.
현수네 반에는 N명의 학생들이 있습니다.
선생님은 반 학생들에게 반 번호를 정해 주기 위해 운동장에 반 학생들을 키가 가장 작은 학
생부터 일렬로 키순으로 세웠습니다. 제일 앞에 가장 작은 학생부터 반 번호를 1번부터 N번까
지 부여합니다. 현수는 짝꿍보다 키가 큽니다. 그런데 현수가 앞 번호를 받고 싶어 짝꿍과 자
리를 바꿨습니다. 선생님은 이 사실을 모르고 학생들에게 서있는 순서대로 번호를 부여했습니
다.
현수와 짝꿍이 자리를 바꾼 반 학생들의 일렬로 서있는 키 정보가 주어질 때 현수가 받은 번
호와 현수 짝꿍이 받은 번호를 차례로 출력하는 프로그램을 작성하세요.
▣ 입력설명
첫 번째 줄에 자연수 N(5<=N<=100)이 주어진다.
두 번째 줄에 제일 앞에부터 일렬로 서있는 학생들의 키가 주어진다.
키(높이) 값 H는 (120<=H<=180)의 자연수 입니다.
▣ 출력설명
첫 번째 줄에 현수의 반 번호와 짝꿍의 반 번호를 차례로 출력합니다.
▣ 입력예제 1
9
120 125 152 130 135 135 143 127 160
▣ 출력예제 1
3 8
출력해설 : 키 정보 152가 현수이고, 127이 현수 짝꿍입니다.
▣ 입력예제 2
6
120 130 150 150 130 150
▣ 출력예제 2
3 5

## 7-7. 좌표 정렬

N개의 평면상의 좌표(x, y)가 주어지면 모든 좌표를 오름차순으로 정렬하는 프로그램을 작성하
세요. 정렬기준은 먼저 x값의 의해서 정렬하고, x값이 같을 경우 y값에 의해 정렬합니다.
▣ 입력설명
첫째 줄에 좌표의 개수인 N(3<=N<=100,000)이 주어집니다.
두 번째 줄부터 N개의 좌표가 x, y 순으로 주어집니다. x, y값은 양수만 입력됩니다.
▣ 출력설명
N개의 좌표를 정렬하여 출력하세요.
▣ 입력예제 1
5
2 7
1 3
1 2
2 5
3 6
▣ 출력예제 1
1 2
1 3
2 5
2 7
3 6

## 7-8. 회의실 배정

한 개의 회의실이 있는데 이를 사용하고자 하는 n개의 회의들에 대하여 회의실 사용표를 만들
려고 한다. 각 회의에 대해 시작시간과 끝나는 시간이 주어져 있고, 각 회의가 겹치지 않게 하
면서 회의실을 사용할 수 있는 최대수의 회의를 찾아라. 단, 회의는 한번 시작하면 중간에 중
단될 수 없으며 한 회의가 끝나는 것과 동시에 다음 회의가 시작될 수 있다.
▣ 입력설명
첫째 줄에 회의의 수 n(1<=n<=100,000)이 주어진다. 둘째 줄부터 n+1 줄까지 각 회의의 정
보가 주어지는데 이것은 공백을 사이에 두고 회의의 시작시간과 끝나는 시간이 주어진다.
회의의 시작시간과 끝나는 시간의 조건은 (시작시간 <= 끝나는 시간)입니다.
▣ 출력설명
첫째 줄에 최대 사용할 수 있는 회의 수를 출력하여라.
▣ 입력예제 1
5
1 4
2 3
3 5
4 6
5 7
▣ 출력예제 1
3
예제설명
(2, 3), (3, 5), (5, 7)이 회의실을 이용할 수 있다.
▣ 입력예제 2
3
3 3
1 3
2 3
▣ 출력예제 2
2

## 7-9. 결혼식

현수는 다음 달에 결혼을 합니다.
현수는 결혼식 피로연을 장소를 빌려 3일간 쉬지 않고 하려고 합니다.
피로연에 참석하는 친구들 N명의 참석하는 시간정보를 현수는 친구들에게 미리 요구했습니다.
각 친구들은 자신이 몇 시에 도착해서 몇 시에 떠날 것인지 현수에게 알려주었습니다.
현수는 이 정보를 바탕으로 피로연 장소에 동시에 존재하는 최대 인원수를 구하여 그 인원을
수용할 수 있는 장소를 빌리려고 합니다. 여러분이 현수를 도와주세요.
만약 한 친구가 오는 시간 13, 가는시간 15라면 이 친구는 13시 정각에 피로연 장에 존재하는
것이고 15시 정각에는 존재하지 않는다고 가정합니다.
▣ 입력설명
첫째 줄에 피로연에 참석할 인원수 N(5<=N<=100,000)이 주어집니다.
두 번째 줄부터 N줄에 걸쳐 각 인원의 오는 시간과 가는 시간이 주어집니다.
시간은 첫날 0시를 0으로 해서 마지막날 밤 12시를 72로 하는 타임라인으로 오는 시간과 가
는 시간이 음이 아닌 정수로 표현됩니다.
▣ 출력설명
첫째 줄에 피로연장에 동시에 존재하는 최대 인원을 출력하세요.
▣ 입력예제 1
5
14 18
12 15
15 20
20 30
5 14
▣ 출력예제 1
2
