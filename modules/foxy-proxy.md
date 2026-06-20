

<p><h1>Install Foxy Proxy</h1></p>

<p>You can find the installation for the foxy proxy web extension here,</p>

https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-basic/

<p>Or you can just use ParrotOS and have it pre-installed for you ;)</p>

<p><h1>Configuring foxy proxy</h1></p>

1. Click on the extension in your browser toolbar
2. Click Options
3. Click Add
4. Title "BURP"
5. Proxy IP: 127.0.0.1
6. 8080
7. Save
8. Click on the foxy proxy icon in your toolbar and select Burp

**<p>Make sure you turn proxy intercept on in burp suite.</p>**

<p>Note, I was unsure why a loopback address was used for the IP Address here.<br>

It turns out that this ensures the proxy only intercepts traffic from the local machine without exposing the proxy to the external network.</p>

