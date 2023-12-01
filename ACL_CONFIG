R1
no access-list 1
access-list 1 permit any
int se0/0/0
ip access-group 1 out

R2
no access-list 1
access-list 1 deny host 192.168.0.2
access-list 1 deny host 192.168.0.3
access-list 1 permit any
int fa0/0
ip access-group 1 out

R3
no access-list 1
access-list 1 deny host 192.168.0.4
access-list 1 deny host 192.168.0.5
access-list 1 deny 192.168.3.0   0.0.0.255
access-list 1 permit any
int fa0/0
ip access-group 1 out
int se0/0/1
ip access-group 1 in
