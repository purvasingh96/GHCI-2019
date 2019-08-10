# Command Injection

# Overview
* Considering a website that is used to ping your ip-address/domain name for.eg. below is a website that would ping the entered ip-address/domain.
<img src="./images/01.sample_pinging_website.png"></img>


# Steps to Perform Command Injection
## Step 1: Login to OWASP 
* Login to OWASP and click on Damn Vulnerable Web Applications 
<img src="./images/02.Damn_vulnerable.png"></img>
* You would be re-directed to DVWA's login page. 
* Login to DVWA using **admin as username and password.**<br>
<img src="./images/03.dvwa_login_page.png"></img>
* Type in sample command such as `whoami` after a **dot and comma (.,)** as below <br>
<img src="./images/05.whoami_example.png"></img>

* In the result, you see the outputs of both commands i.e. **ping and whoami.**<br>
<img src="./images/04.command_injection_done.png"></img>

# Exploiting Command Injection
* We can try to make a connection with DVWA's machine to our Kali Linux Machine. This can be done using `netcat`
* `netcat` is used to connect 2 PCs
    * For our Kali linux, we need to set up **listening port,** e.g.12345
        * Type the following command `nc -lvp 12345`
        * -l is listening mode
        * -v is verbose mode
        * -p specifies port number<br>
        <img src="./images/05.listening_port.png"></img>
    *  Listening port would be used to listen to any connection coming to our PC.
     
