# 리눅스 명령어 (top,ps,jobs,kill 명령어)

20233158이동헌
***

## 차례
- top 명령어
- ps 명령어
- jobs 명령어
- kill 명령어

***

### top명령어

**Top 명령어란?**

실시간으로 CPU 사용률을 체크해주는 도구이다. 리눅스를 사용하는 서버의 성능이나 현재 돌아가고 있는 상황을 볼 때 사용한다.

**사용법?**

리눅스에서 top 명령어를 치고 들어가면? 끝!
root#> top

명령어를 치고 들어가면? 아래와 같은 화면을 볼 수 있다.


![image](https://github.com/dlehdgjs/saka/assets/133830046/6fa9543c-9a2f-46bc-adc5-268832418099)

**top 실행 후 명령어**

-> shift+p : CPU 사용률 내림차순

-> shift+m : 메모리 사용류 내림차순

-> shift+t : 프로세스가 돌아가고 있는 시간 순

-> k : kill,k 입력 후 PID 번호 작성, signal은 9

-> a : 메모리 사용량에 따라 정령

-> b : Batch 모드로 작동

-> 1 : CPU Core별로 사용량 보여줌

***

### ps 명령어

**ps 명령어란?**

리눅스에는 여러 개의 프로세스가 동시에 실해되기 때문에 실행 중인 프로세스의 정보를 얻기 위해 사용되는 명령어이다.

***프로세스 중에서 CPU, 메모리 등등을 많이 점유하고 있거나, 지나치게 많은 지식 프로세스를 생성하는 등에 시스템에 속도가 느려지는 경우 PS 명령어로 분석하여 시스템 오류를 감지할 수 있다.***


**사용법**

-> ps


![image](https://github.com/dlehdgjs/saka/assets/133830046/37c64726-2261-4e5d-808a-8023eab50bc8)



-> ps-ef | grep abc : abc가 포함된 라인들 출력

-> ps-f : 전체 포맷으로 출력

-> ps-l : 긴 포맷으로 출력

-> ps-p : 프로세스 번호

-> ps-e : 모든 프로세스 출력

-> ps-ef | more : 모든 프로세스를 전체 포맷으로 출력


***

### ps와 top의 차이점

- ps는 ps한 시점에 proc에서 검색한 cpu 사용량을 출력한다.

- top은 proc에서 일정 주기로 합산해 cpu 사용율을 출력한다.


### jobs









