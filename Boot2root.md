Boot2root

My ip :  192.168.56.1
Target ip : 192.168.56.101


NMAP SCAN :

Nmap scan report for 192.168.56.101
Host is up (0.000039s latency).
Not shown: 994 closed tcp ports (reset)
PORT    STATE SERVICE    VERSION
21/tcp  open  ftp        vsftpd 2.0.8 or later
|_ftp-anon: got code 500 "OOPS: vsftpd: refusing to run with writable root inside chroot()".
22/tcp  open  ssh        OpenSSH 5.9p1 Debian 5ubuntu1.7 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   1024 07bf0220f08ac8481efc41aea446fa25 (DSA)
|   2048 26dd80a3dfc44b531e534246ef6e30b2 (RSA)
|_  256 cfc38c31d7477c84e2d21631b28e63a7 (ECDSA)
80/tcp  open  http       Apache httpd 2.2.22 ((Ubuntu))
|_http-title: Hack me if you can
|_http-server-header: Apache/2.2.22 (Ubuntu)
143/tcp open  imap       Dovecot imapd
|_imap-capabilities: OK more STARTTLS have post-login capabilities listed ID LOGIN-REFERRALS Pre-login IDLE LITERAL+ IMAP4rev1 ENABLE LOGINDISABLEDA0001 SASL-IR
|_ssl-date: 2024-11-29T16:09:07+00:00; -1s from scanner time.
443/tcp open  ssl/http   Apache httpd 2.2.22
|_http-title: 404 Not Found
|_ssl-date: 2024-11-29T16:09:07+00:00; -1s from scanner time.
| ssl-cert: Subject: commonName=BornToSec
| Not valid before: 2015-10-08T00:19:46
|_Not valid after:  2025-10-05T00:19:46
|_http-server-header: Apache/2.2.22 (Ubuntu)
993/tcp open  ssl/imaps?
|_ssl-date: 2024-11-29T16:09:07+00:00; -1s from scanner time.
| ssl-cert: Subject: commonName=localhost/organizationName=Dovecot mail server
| Not valid before: 2015-10-08T20:57:30
|_Not valid after:  2025-10-07T20:57:30
MAC Address: 08:00:27:7A:6B:B2 (Oracle VirtualBox virtual NIC)
Service Info: Host: 127.0.1.1; OS: Linux; CPE: cpe:/o:linux:linux_kernel


http://192.168.56.101 => Hack me website with one subdirectory 192.168.56.101/fonts