# open_homework
## ***리눅스 명령어***
### [top]
> top -b: 배치모드로 정보를 출력한다. 실시간 상화 대화형모드로 정보를 화면에 일렬로 출력한다.
> 
> top -d delay: 지정한 시간(delay 초)의 간격으로 정보를 업데이트하여 출력한다.
> 
> top -i idle: 토글값이 off일 때, idle 프로세스나 좀비 프로세스 정보를 출력하지 않는다.
> 
> top -n num: 지정한 시간(num)만큼 업데이트 정보를 출력한다.
> 
> top -p pid: 지정한 프로세스 ID(pid)의 정보만을 출력한다.
> 
> top -q: 시간의 간격 없이 계속하여 업데이트 정보를 출력한다.
> 
> top -s: 몇 개의 대화식 명령을 비활성화한다(시큐어 모드).
> 
> top -S: 누적된 정보를 출력한다(cumulative 모드).
> 

### [ps]
***전체 프로세스와 관련된 옵션***
> ps -A: 모든 프로세스를 출력한다.
> 
> ps -N : -A 옵션과 비슷하나 ps 프로세스를 제외하고 출력한다.
> 
> ps -a : 세션 리더 및 터미널에 속하지 않는 프로세스를 제외하고 출력한다.
> 
> ps -d : 세션 리더를 제외한 모든 프로세스를 출력한다.
> 
> ps -e : 커널 프로세스를 제외한 모든 프로세스를 출력한다.
> 
> ps T : 현재 터미널에서의 모든 프로세스를 출력한다.
> 
> ps a : 현재 터미널의 사용자 고유 프로세스를 출력한다.
> 
> ps r : 현재 실행 중인 프로세스를 출력한다.
> 
> ps x : 터미널이 없는 프로세스를 출력한다.
> 
> ps --deselect : -N 옵션과 같다.

***특정 프로세스를 선택하여 보여주는 옵션***
> ps -C : 지정한 명령어의 이름에 관련된 정보를 출력한다.
>
> ps -G : 그룹 ID에 관련된 정보를 출력한다(이름도 지원).
>
> ps -U : 사용자 ID에 관련된 정보를 출력한다(이름도 지원).
>
> ps -g : 지정한 세션 리더 혹은 그룹명에 관련한 정보를 출력한다.
>
> ps -p : 프로세스 ID를 출력한다.
>
> ps -s : 세션에 속한 프로세스를 지정한다.
>
> ps -t : tty를 지정한다.
>
> ps -u : 사용자 ID를 지정한다(이름도 지원).
>
> ps U : 지정한 사용자의 프로세스를 출력한다.
>
> ps p : 프로세스 ID를 지정한다.
> 
> ps t : tty를 지정한다.
> 
> ps --Group : 실제 그룹 이름이나 ID를 지정한다.
> 
> ps --User : 실제 사용자 이름이나 ID를 지정한다.
> 
> ps --group : 유효 사용자 이름이나 ID를 지정한다.
> 
> ps --pid : 프로세스 ID를 지정한다.
> 
> ps --sid : 세션 ID를 지정한다.
> 
> ps --tty : 터미널을 지정한다.
> 
> ps --user : 유효 사용자 이름이나 ID를 지정한다.
> 
> ps -123 : --sid 123과 같은 의미이다.
> 
> ps 123 : --pid 123과 같은 의미이다.

***출력 결과 필드를 제어하는 옵션***
> ps -0 : PID, TTY, STAT, TIME, COMMAND 등의 필드 목록을 출력한다.
> 
> ps -c : PID, CLS, PRI, TTY, TIME. CMD 등의 필드 목록을 출력한다.
> 
> ps -f : UID, PID, PPID, C, STIME, TTY, TIME, CMD 등의 필드를 CMD 필드의 전체 명령어 형태로 출력한다.
> 
> ps -j : PID, PGID, SID, TTY, TIME, CMD 등의 필드 목록을 출력한다.
> 
> ps -l : F, S, UID, PID, PPID, C, PRI, NI, ADDR, SZ, WCHAN, TTY, TIME, CMD 필드의 상세 정보를 출력한다.
> 
> ps -o : 사용자가 정의한 포맷을 지정한다.
> 
> ps -y : -l 이나 l 옵션과 함께 ADDR 필드를 RSS 필드로 출력한다.
> 
> ps 0 : PID, TTY, STAT, IME COMMAND 필드 정보를 출력한다.
> 
> ps X : PID, STACKP, ESP, EIP, TMOUT, ALARM, STAT, TTY, TIME, COMMAND 필드의 정보를 리눅스 i386 레지스터 형식으로 출력한다.
> 
> ps j : PPID, PID, PGID, SID, TTY, TPGID, STAT, UID, TIME, COMMAND 필드의 정보를 작업 제어에 관련된 형식으로 출력한다.
> 
> ps l : F, S, UID, PID, PPID, C, PRI, NI, ADDR, SZ, PSS, WCHAN, TTY, TIME, CMD 필드의 정보를 출력하고 -l 옵션과 함께 PSS 필드를 추가하여 출력한다.
> 
> ps o : 사용자 지정 형식으로 출력한다.
> 
> ps s : UID, PID, PENDING, BLOCKED, IGNORED, CAUGHT, STAT, TTY, TIME, COMMAND 필드의 정보를 출력한다.
> 
> ps u : USER, PID, %CPU, %MEM, VSZ, RSS, TTY, STAT, START, TIME, COMMAND 필드의 정보를 출력한다.
> 
> ps v : PID, TTY, STAT, TIME, MAJFL, TRS, DRS, RSS, %MEM, COMMAND 필드의 정보를 출력한다.
> 
> ps --format : 사용자 지정 형식으로 출력한다.

***출력 필드의 내용을 변경하는 옵션***
> ps -H : 프로세스를 계층형으로 출력한다.
> 
> ps -m : 스레드 정보를 출력한다.
> 
> ps -n namelist : 시스템 이름 리스트 파일(namelist)을 지정한다.
> 
> ps -w : 너비에 맞게 잘려진 내용을 제한이 없는 너비의 내용으로 상세하게 출력한다.
> 
> ps --cols : 스크린의 너비를 설정한다.
> 
> ps --columns : 스크린의 너비를 설정한다.
> 
> ps --cumulative : 죽은 자식 프로세스 데이터를 포함하여 출력한다.
> 
> ps --forest : 아스키 문자의 프로세스 트리 형태로 출력한다.
> 
> ps --html : HTML 이스케이프로 출력한다.
> 
> ps --headers : 헤더 라인을 반복한다.
> 
> ps --no-headers : 헤더를 보이지 않는다.
> 
> ps --lines : 스크린의 높이를 설정한다.
> 
> ps --rows : 스크린의 높이를 설정한다.
> 
> ps --sort : 정렬 방식을 지정한다.
> 
> ps C : CPU 시간을 이용한다.
> 
> ps N : 지정한 시스템 이름의 리스트 파일을 사용한다.
> 
> ps O : 정렬 순서 지정하기 위한 옵션으로 O[+|-]K[,[+|-]K[,···]]의 형식으로 지정한다. +는 오름차순 정렬, –는 내림차순 정렬이다.
> 
> ps S : 죽은 자식 프로세스의 데이터를 포함한다.
> 
> ps c : 시스템 내부에 보관 중인 명령어 이름을 출력한다.
> 
> ps e : 명령어에 대한 매개 변수와 함께 환경 변수를 출력한다.
> 
> ps f : 아스키(*) 아트로 프로세스 트리를 출력한다.
> 
> ps h : 헤더 라인은 출력하지 않는다.
> 
> ps m : 모든 스레드 정보를 출력한다.
> 
> ps n : WCHAN과 USER 필드를 숫자 값으로 출력한다.
> 
> ps w : 필드의 너비에 맞게 잘려진 내용을 너비보다 상세하게 출력한다.
> 
> ps --cols : 스크린의 너비를 설정한다.
> 
> ps --columns : 스크린의 너비를 설정한다.
> 
> ps --cumulative : 죽은 자식 프로세스 데이터를 포함한다.
> 
> ps --forest : 아스키 아트의 프로세스 트리를 출력한다.
> 
> ps --html : HTML 이스케이프를 출력한다.
> 
> ps --headers : 헤더 라인을 반복한다.
> 
> ps --no-headers : 헤더를 출력하지 않는다.
> 
> ps --lines : 스크린의 높이를 설정한다.
> 
> ps --rows : 스크린의 높이를 설정한다.
> 
> ps --sort : 지정한 정렬 방식으로 출력한다.
> 
> ps --sort＝[+|-]key[,[+|-]key[,···] 형식이다. 

***프로그램의 정보***
> ps -V : 버전 정보를 출력한다.
> 
> ps L : 모든 형태의 지시자를 출력한다.
> 
> ps V : 버전 정보를 출력한다.
> 
> ps --help : 사용법을 출력한다.
> 
> ps --info : 디버깅 정보를 출력한다.
> 
> ps --version : 버전 정보를 출력한다.

### [jobs]
***쓰는 방법***

***jobs [옵션][jobID...]***

***jobs -x command [args]***
>-l : 프로세스 그룹 ID를 state 필드 앞에 출력한다.
>
>-n : 프로세스 그룹 중에 대표 프로세스 ID를 출력한다.
>
>-p : 각 프로세스 ID에 대해 한 행씩 출력한다.
>
>command : 지정한 명령어를 실행한다.

***확인할 수 있는 세션의 상태값
|상태|설명|

### [kill]
