

<p><h1>Task: Investigate the site http://10.66.176.29/</h1></p>

<p>First I clicked into the target tab and defined the scope, which is 10.66.176.29 in this case.<br>
I then went to the proxy tab and turned intercept on.</p>

<p>From here I just clicked on every tab available on the website to gather all the information I could.<br>
On the contact and ticket forms I threw some SQL queries in there just for fun and to see if anything came up.</p>

```
SHOW DATABASES;
SHOW TABLES;
SELECT * FROM;
```

<p>I then went back to the Target Tab --> Site Map, and reviewed all the different paths available.<br>
Upon review, I noticed a path with randomized characters that seemed way different from the rest.<br>
This ended up being our flag value.</p>

http://10.66.176.29/ticket/
http://10.66.176.29/5yjR2GLcoGoij2ZK

```
THM{NmNlZTliNGE1MWU1ZTQzMzgzNmFiNWVk}
```

<p><h1>Other observations,</h2></p>

<p>This server is running nginx/1.18.0 (Ubuntu) using the outdated HTTP/1.1 protocol.</p>

<p>NGINX 1.18.0 has multiple known vulnerabilities, including CVE-2026-42945, which allows an unauthenticated attacker to crash a worker process or potentially achieve remote code execution</p>
