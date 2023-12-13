# Build your own DNS server (Python)
https://app.codecrafters.io/courses/dns-server/overview

---

### Start server

`python -m app.main`

---

### Test manually with dig 

`dig @127.0.0.1 -p 2053 codecrafters.io`

```
; <<>> DiG 9.10.6 <<>> @127.0.0.1 -p 2053 codecrafters.io
; (1 server found)
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 58909
;; flags: qr rd; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 0
;; WARNING: recursion requested but not available

;; QUESTION SECTION:
;codecrafters.io.		IN	A

;; ANSWER SECTION:
codecrafters.io.	60	IN	A	8.8.8.8

;; Query time: 0 msec
;; SERVER: 127.0.0.1#2053(127.0.0.1)
;; WHEN: Wed Dec 13 08:53:00 CST 2023
;; MSG SIZE  rcvd: 64
```
