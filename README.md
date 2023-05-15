# Computer_Structure_Finalexam
컴퓨터구조 기말고사 정리입니다.

![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/8e9000b9-80cf-4e01-ae6a-0e5031b7e8c8)
```
1번 문제 풀이

average rotational latency 즉 회전 지연 시간을 구하는 문제이다.
0.5rotation/(7,200/60RPS) = 4.167 (아마 근삿값으로 오차도 허용)

transfer time 데이터에 접근해서 데이터를 전송하는데 걸리는 시간 거/속*시, 즉 transfer rate 속도가 34MB/sec 로 주어졌고 거리는 1024byte = 1KB로 주어져있으니까 시간은 거/속 1KB/(34MB/sec) = 0.029ms(오차범위허용) 1/34 해준 값임

controller overhead : 문제에서 주어진 480 Mbits/sec을 물리단위 변환하라는 문제 1byte는 8bit니까 (480*M/8)/sec 계산하면 
60MB/sec 를 ms로 변환하면 1/60 하라는 거 그래서 0.017ms

4개 (average rotational latency + transfer time + controller overhead + average seek time) 다 더하면
4.167 + 0.029 + 0.017 + 11 = 15.206 
```
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/4a3405aa-d429-4cf1-b5ac-4b7bd2b177a5)
```
2번 문제 풀이
```
