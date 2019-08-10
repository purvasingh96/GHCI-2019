# Command Injection

# Overview
* Considering a website that is used to ping your ip-address/domain name for.eg. below is a website that would ping the entered ip-address/domain.
<img src="./images/01.sample_pinging_website.png"></img>


# Steps to Perform Command Injection
## Step 1: Login to OWASP 
* Login to OWASP and click on Damn Vulnerable Web Applications 
<img src="./images/02.Damn_vulnerable.png"></img>
* You would be re-directed to DVWA's login page. 
* Login to DVWA usinf **admin as username and password.**<br>
<img src="./images/03.dvwa_login_page.png"></img>
* Type in sample command such as `whoami` after a **dot and comma (.,)** as below <br>
<img src="./images/05.whoami_example.png"></img>

* In the result, you see the outputs of both commands i.e. **ping and whoami.**<br>
<img src="./images/04.command_injection_done.png"></img>
