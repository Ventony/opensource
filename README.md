# Linux 명령어 이해하기
## top 명령어는 리눅스에서 시스템 성능을 실시간으로 모니터링하는 강력한 도구입니다.
## CPU, 메모리 사용량 및 실행 중인 프로세스의 동적 요약을 표시하여 시스템 리소스를 관리하고 성능을 최적화하는 데 도움이 됩니다.

### 목차
1. 소개
2. top 명령어 사용 방법
3. Top 명령어 섹션
   * 요약 영역
   * 상세 영역
4. 상호 작용 명령어
5. 결론
### 소개
top 명령어는 시스템의 성능을 모니터링하기 위해 사용되며, CPU, 메모리 사용량, 실행 중인 프로세스에 대한 실시간 데이터를 제공합니다.
시스템 관리자가 성능 조정 및 문제 해결을 위해 매우 중요한 명령어입니다.

### top 명령어 사용 방법
top 명령어를 시작하려면, 터미널에서 간단히 다음 명령을 입력합니다: top
이 명령을 실행하면 실시간으로 업데이트되는 시스템의 현재 상태를 볼 수 있습니다.

### Top 명령어 섹션
#### 요약 영역
요약 영역에는 시스템의 전반적인 상태에 대한 정보가 포함됩니다. 여기에는 다음과 같은 항목이 포함됩니다:

* 시스템 시간: 현재 시스템의 시간입니다.
* 업타임: 시스템이 부팅된 후 경과한 시간입니다.
* 사용자 수: 현재 시스템에 로그인한 사용자 수입니다.
* 로드 평균: 1분, 5분, 15분 간의 평균 부하를 나타냅니다.
  
### 상세 영역
상세 영역에는 개별 프로세스에 대한 정보가 나열됩니다. 여기에는 다음과 같은 항목이 포함됩니다:
* PID: 프로세스 ID입니다.
* USER: 프로세스를 실행한 사용자입니다.
* PR: 프로세스의 우선순위입니다.
* NI: 프로세스의 nice 값입니다.
* VIRT: 프로세스가 사용 중인 가상 메모리의 크기입니다.
* RES: 프로세스가 사용 중인 실제 메모리의 크기입니다.
* SHR: 프로세스가 사용하는 공유 메모리의 크기입니다.
* S: 프로세스의 상태입니다 (e.g., S: Sleep, R: Running).
* %CPU: 프로세스가 사용하는 CPU의 비율입니다.
* %MEM: 프로세스가 사용하는 메모리의 비율입니다.
* TIME+: 프로세스가 사용한 총 CPU 시간입니다.
* COMMAND: 실행된 명령어입니다.
  
### 상호 작용 명령어
top 명령어 실행 중에 다양한 키를 눌러 정보를 제어할 수 있습니다:
* h: 도움말 메뉴를 엽니다.
* k: 특정 프로세스를 종료합니다.
* r: 특정 프로세스의 우선순위를 변경합니다.
* q: top 명령어를 종료합니다.

### 결론
top 명령어는 리눅스 시스템의 성능을 실시간으로 모니터링할 수 있는 강력한 도구입니다. 시스템 관리자에게 매우 유용하며, CPU 및 메모리 사용량을 최적화하고 문제를 해결하는 데 도움을 줍니다.

## ps 명령어는 현재 시스템에서 실행 중인 프로세스의 상태를 확인하는 데 사용됩니다.
## 이는 프로세스의 스냅샷을 제공하며, 다양한 옵션을 통해 원하는 정보를 상세히 볼 수 있습니다.

### 목차
1. 소개
2. ps 명령어 사용 방법
3. ps 명령어 옵션
   * UNIX 계열 옵션
   * BSD 계열 옵션
4. 자주 사용하는 예시
5. 결론
   
### 소개
ps 명령어는 "Process Status"의 약자로, 현재 실행 중인 프로세스의 상태를 보여줍니다. 이는 시스템 모니터링 및 관리에 필수적인 도구입니다.

### ps 명령어 사용 방법
터미널에서 ps 명령어를 입력하면 기본적으로 현재 셸에서 실행 중인 프로세스 목록이 출력됩니다: ps
### ps 명령어 옵션
#### UNIX 계열 옵션
* -e : 실행 중인 모든 프로세스를 출력
* -f : 풀 포맷으로 리스트를 출력
* -l : 더 자세한 정보를 출력
#### BSD 계열 옵션
* a : 터미널과 연관된 모든 프로세스를 출력
* u : 프로세스의 소유자를 기준으로 출력
* x : 터미널과 연관되지 않은 프로세스도 출력
   
### 자주 사용하는 예시
* ps -ef
모든 실행 중인 프로세스를 풀 포맷으로 출력: ps -ef

* ps aux
BSD 스타일로 모든 프로세스를 출력: ps aux

### 결론
ps 명령어는 리눅스 시스템의 프로세스를 모니터링하고 관리하는 데 중요한 도구입니다. 다양한 옵션을 사용하여 필요한 정보를 쉽게 얻을 수 있습니다.

## jobs 명령어는 현재 셸 세션에서 실행 중인 백그라운드 및 포어그라운드 작업을 표시합니다.
## 작업을 모니터링하고 관리하는 데 유용합니다.

### 목차
1. 기본 사용법
2. 옵션
3. 예시
   
### 기본 사용법
이 명령어는 현재 셸에서 실행 중인 모든 작업을 표시합니다: jobs

### 옵션
* -l: 각 작업의 프로세스 그룹 ID를 함께 표시합니다.
* -p: 각 작업의 프로세스 ID만 표시합니다.
* -n: 최근에 상태가 변경된 작업만 표시합니다.
  
#### 기본 사용: jobs
#### 프로세스 그룹 ID 표시: jobs -l
#### 프로세스 ID 표시: jobs -p

## kill 명령어는 특정 프로세스에 시그널을 보내는 데 사용되며,
## 주로 프로세스를 종료하는 데 사용됩니다.

### 목차
1. 기본 사용법
2. 시그널
3. 예시
   
### 기본 사용법
PID는 종료하려는 프로세스의 ID입니다: kill [옵션] <PID>

### 시그널
* -15 (SIGTERM): 프로세스를 정상적으로 종료합니다. (기본값)
* -9 (SIGKILL): 프로세스를 강제로 종료합니다.
* -1 (SIGHUP): 프로세스를 다시 로드합니다.
  
#### 기본 종료: kill 1234
#### 강제 종료: kill -9 1234
#### 프로세스 다시 로드: kill -1 1234
