

<p><h1>Task: Successfully exploit the web application using XSS</h1></p>

```
TARGET:http://10.66.176.29/ticket/
```

<p>First we should go to target--> scope --> Add URL to add our target URL<br>
After we add our URL we should go to proxy --> proxy settings --> and enable the "in scope" checkboxes.<br>
This will prevent us from receiving junk output.</p>

<p>We can now test if these user-input prompts are vulnerable to XSS.</p>

![landing-page](https://github.com/ch1c4g0/learn-burp-suite/blob/e0da7ff1d0379a9044334a59189a5e8802d156c4/screenshots/2026-06-20_11-18.png)

<p>I first tested box two "type your query here",</p>

```
<script>alert("REFLECT THIS PAL")</script>
```

<p>I used alert to see if an alert would pop-up in the browser (you'll see later if your unsure), but nothing was returned.

<p>The email address prompt did not allow special characters, to bypass this, we'll send a "legitimate" query with our proxy enabled, then edit the email address field.<br>
We can now insert our script from above, we need to make sure before we forward the modified query that we URL encode the data, otherwise, this will not work.</p>

![modified-query-example](https://github.com/ch1c4g0/learn-burp-suite/blob/65cc7303a60a50d53247e8aa2e91ebe3988db688/screenshots/2026-06-20_11-32.png)

<P>After we encode the data (Ctrl+U) we can forward our query.</P>

<p><h1>Success!</h1></p>

![successful-xss](https://github.com/ch1c4g0/learn-burp-suite/blob/455e8f9a65721e3e066342d245bb44de713742b2/screenshots/2026-06-20_11-37.png)
