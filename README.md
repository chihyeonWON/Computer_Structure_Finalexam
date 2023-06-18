# Computer_Structure_Finalexam
컴퓨터구조 기말고사 정리입니다.

## 기말고사 풀이
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/8f9a5f6e-bae1-43f8-99f4-03aadff811f8)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/5faa42bc-bca1-488c-a32d-4b7cea629e2d)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/f864dc2a-c0fc-4999-af25-7726efbe02ba)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/35b614a9-a562-4acb-9372-df355a246af3)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/f8b6c360-f3bf-4205-9619-d8a77d0be1c0)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/5c64bf74-c52e-4a64-b541-eba84965c255)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/8fe062b0-2ed2-4cf8-b87e-377caa778a61)



[기말고사 정리는 여기서](https://ttl-blog.tistory.com/1096)
[데이터 Harzard Forwarding](https://velog.io/@embeddedjune/%EC%BB%B4%ED%93%A8%ED%84%B0%EA%B5%AC%EC%A1%B0-%EC%9A%94%EC%95%BD-%EC%A0%95%EB%A6%AC-9.-Pipelined-Architecture-3)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/8e9000b9-80cf-4e01-ae6a-0e5031b7e8c8)
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/aa950302-63f2-4750-9435-37404912f2a3)


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
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/84f9b370-a5db-4aaa-9266-321e039ed600)
```
1번 문제 풀이

block 개수 = (32K/2)/8 = 2K = 2의 11승 
index size = 11
tag size = 64-(11+1+3) = 49

valid + tag = metadata
total cache size = #blocks * (valid + tag + data) = 2의11 * (1 + 49 + 2*64)

block 개수 = (64K/16)/8 = 0.5K = 2의 9승
index size = 9
tag size = 64-(9+4+3) = 48
total cache size = 2의9 * (1 + 48 + 16*64) = 549376 (콤마 쓰지 말것)
```
![image](https://github.com/chihyeonWON/Computer_Structure_Finalexam/assets/58906858/1a3afc56-e893-498c-bcaa-2795e32b010f)
```
2번 문제 풀이

문제 오류로 생략
```
