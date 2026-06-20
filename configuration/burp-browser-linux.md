

<p>Upon attempting to open the burp browser you will most likely encounter a sandboxing error.<br>
To use burp browser it is recommended to create a non-privileged user, then run burp suite under that user.</p>

```
Smart option: Create a new user and run Burp Suite under a low-privilege account to allow the Burp Browser to run without issues.
Easy option: Go to Settings -> Tools -> Burp's browser and check the Allow Burp's browser to run without a sandbox option.
Enabling this option will allow the browser to start without a sandbox, please be aware that this option is disabled by default for security reasons.
If you choose to enable it, exercise caution, as compromising the browser could grant an attacker access to your entire machine.
In the training environment of the AttackBox, this is unlikely to be a significant issue, but use it responsibly.
```
