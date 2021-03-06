> - 이곳은 해당 주차에 문제를 풀면서 알게된 노하우 / 정보를 공유하는 공간입니다.
> - 노하우 / 정보 뿐만 아니라 해당 문제를 풀면서 어려웠던 점이나 자유로운 코멘트를 추가하여도 좋습니다 :)
> - [마크다운 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)

## Todo
    - 알고리즘 분석
    - 링크드 리스트 구현

## Tips
- 강필규
    - (예시) 1번
        - a <= X <= b 방식의 표현보다 a <= X < b 같은 범위 표현 방법이 유리한 점이 많습니다.
    - 백준_1158번 (조세퍼스)
        - 시간복잡도 O(nk) -> 사람 수 N * K 번째 포인터
        - (K-1) mod N번 위치로 계산을 줄이는 경우도 존재한다. 보통 N > K 인 경우 유리 -> 해당 시간 복잡도 O(n^2)
    - 백준_2406 (에디터)
        - 특별한 알고리즘 로직 해결방안이 없는거 같아 말 그대로 문제 해결
        - JAVA 시간초과 (제한 2초)
        - Scanner Class vs BufferedReader 성능 비교...
        - BufferedReader가 읽어들이는 속도가 빠름
        - 빠른 이유 : 한 줄씩 버퍼로 읽어들이기에 한 문자 단위로 읽어오는 Scanner 보다 빠르다.
        - 언제 사용 : 알고리즘 문제에서 한 줄에 큰 사이즈에 입력값이 주어지는 경우 BufferedReader 사용하는 것이 거의 필수적
    - 백준_2983 (개구리 공주)
        - N 개의 입력값을 받지만 시작점과 비교해 보았을 경우 이동할 수 있는 점들 값이 결정됨..(x+y % 2 이 같아야한다.) -> N 수 자체를 줄일 수 있음..
        - 한 점을 기준으로 대각선으로만 움직이기 때문에 X+Y, X-Y 값이 같은 곳으로만 이동 가능하다.
        - X+Y / X-Y 두 값으로 인덱싱할 수 있도록 두 개의 HashSet으로 관리 -> 단점 : 점을 삭제할 경우 동기화가 필요함
- 유준혁
    - 백준_1158번
        - 문제 설명을 이해를 못했어서 혹시나 설명이 필요한 사람을 위해!
        - N까지의 List 각 요소들이 몇 번째에 쫓겨나는 지가 아니라
        - 첫번째 쫓겨나는 친구들 부터 차례대로 출력해주면 된다.
        - 1,2,3,4,5,6,7 로 예를 들면
        - [3]/1,2,index,4,5,6,7 //3이 먼저 출력 되고 남은 List
        - [3,6]/1,2,4,5,index,7 //index로부터 3번째였던 6이 출력되고 다시 그 위치가 index
        - [3,6,2]/1,index,4,5,7 //원형 리스트 이므로 index,7,1,2 이니까 2가 출력. 이런식으로 출력하면 된다.
- 이향아
- 신정연
- 송문준

## Progress
- 강필규 : 백준_1158번, 백준_2406번, 백준_2983번
- 유준혁 : 백준_1158번, 백준_1406번
- 이향아 :
- 신정연 :
- 송문준 :
