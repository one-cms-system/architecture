CREATE CONTROLFILE SET DATABASE orcl LOGFILE GROUP 1 ('/u01/oracle/prod/redo01_01.log', '/u01/oracle/prod/redo01_02.log'), GROUP 2 ('/u01/oracle/prod/redo02_01.log', '/u01/oracle/prod/redo02_02.log'), GROUP 3 ('/u01/oracle/prod/redo03_01.log', '/u01/oracle/prod/redo03_02.log') RESETLOGS DATAFILE '/u01/oracle/prod/system01.dbf' SIZE 3M, '/u01/oracle/prod/rbs01.dbs' SIZE 5M, '/u01/oracle/prod/users01.dbs' SIZE 5M, '/u01/oracle/prod/temp01.dbs' SIZE 5M MAXLOGFILES 50 MAXLOGMEMBERS 3 MAXLOGHISTORY 400 MAXDATAFILES 200 MAXINSTANCES 6 ARCHIVELOG;

create database orcl user sys identified by sys user system identified by system controlfile reuse logfile GROUP 1 ('/u01/oracle/orcl/orcl_g1.rdo') size 10M, GROUP 2 ('/u01/oracle/orcl/orcl_g2.rdo') size 10M, GROUP 3 ('/u01/oracle/orcl/orcl_g3.rdo') size 10M character set WE8ISO8859P15 datafile '/u01/oracle/orcl/orcl_SYSTEM_TS_1.dbf' size 500M autoextend off extent management local default temporary tablespace TEMP tempfile '/u01/oracle/orcl/orcl_TEMP_TS_1.dbf' size 200M autoextend off extent management local uniform size 256K undo tablespace UNDOTBS1 datafile '/u01/oracle/orcl/orcl_UNDOTS_TS_1.dbf' size 200M autoextend off noarchivelog SYSAUX DATAFILE 'd:oracledb01datafilessysaux01.db' SIZE 120M;


sudo iptables -A INPUT -p tcp --dport 1521 -m conntrack --ctstate NEW,ESTABLISHED -j ACCEPT
sudo iptables -A OUTPUT -p tcp --sport 1521 -m conntrack --ctstate ESTABLISHED -j ACCEPT


data:
dbHost: 172.19.20.20
dbPassword_application-service: bXNfYXBwbGljYXRpb24=
dbPassword_authentication-service: ZnNkZ3MyNTE1IWFz
dbPassword_common-service: YmFmYTEyIWFxd3o=
dbPassword_contract-service: dmFlITJkZnMkcw==
dbPassword_education-service: bmFBd3IhczQ1ISQ=
dbPassword_employee-service: YnNzZSFAMjNxYXM=
dbPassword_employer-service: YXNkMjNxcyEyckE=
dbPassword_forwarding-service: dmFzJCFxMTJlYVRk
dbPassword_iep-service: eWJiZCFAMTJhQUR6
dbPassword_person-service: amhBU0Q0MjEhMTQ=
dbPassword_questionnaire-service: amJzUUFEMjIzQDEh
dbPassword_rac-service: bnNkZlpYQzQyISQ=
dbPassword_vacancy-service: TUZEYXdyKDAhNDc=
dbPort: MTUyMQ==
dbSid: b3JjbAo=
dbUsername_application-service: bXNfYXBwbGljYXRpb24=
dbUsername_authentication-service: bXNfYXV0aGVudGljYXRpb24K
dbUsername_common-service: bXNfY29tbW9u
dbUsername_contract-service: bXNfY29udHJhY3Q=
dbUsername_education-service: bXNfZWR1Y2F0aW9u
dbUsername_employee-service: bXNfZW1wbG95ZWU=
dbUsername_employer-service: bXNfZW1wbG95ZXI=
dbUsername_forwarding-service: bXNfZm9yd2FyZGluZw==
dbUsername_iep-service: bXNfaWVw
dbUsername_person-service: bXNfcGVyc29u
dbUsername_questionnaire-service: bXNfcXVlc3Rpb25uYXJpZQ==
dbUsername_rac-service: bXNfcmFj
dbUsername_vacancy-service: bXNfdmFjYW5jeQ==
