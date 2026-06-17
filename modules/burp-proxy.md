
<p><h1>What does Burp Proxy do?</h1></p>

<p>Enalbes capture of requests and responses between the user and the target web server.<br>
This intercepted traffic can be manipulated, sent to other tools, or allowed to reach its destination.</p>

<p><h2>What is the proxy doing?</h2></p>

<p>When intercepting traffic, the packets are held back from reaching their destination.<br>
This allows for manipulation of packets, if you want data to be forwarded turn intercept on.</p>

<p><h3>In proxy settings,</h3></p>

<p>I'd recommend you enable the "Or Request was intercepted" in the response interception rules.<br>
This allows more flexible response interception(more data for you!)</p>

<p><h2>Match and Replace</h2></p>

<p>This allows you to modify incoming and outgoing requests dynamically such as the user-agent or cookies.</p>

