# CSRF
__________________________________________

Just a simple html page to explore a basic csrf vulnerability
__________________________________________


CSRF: Cross Site Request Forgery is a vulnerability where it is possible to change some value or deauthenticate the user just by making him click on a link

Example:

The Facebook target has a login page, where it has 2 functionalities: Enter your email and password and after that (**Already authenticated**) you have the option to change your password.

This glitch occurs when the attacker's server makes a request (can be using basic html) and sends a new password to the target server (the user needs to be authenticated on the target), then after the user clicks on the link, his password will be changed , here is an example of an intentional server error

![image](https://github.com/Gutierre0x80/CSRF/assets/63872706/82b674fe-2e65-477b-be88-aebb95ecc63a)

Read more at https://portswigger.net/web-security/csrf

<h3>How to use</h3>

Configure the page.

Set target and endpoint which has password reset function: 

![image](https://github.com/Gutierre0x80/CSRF/assets/63872706/2eff102f-e4c2-44dd-8ae8-76ddc8cc90da)

Finally, set the email (there is a script that will send the request automatically, but feel free to remove it, the only difference is that the target user will need to enter the email manually. Of course, you need to modify the entry of password ) and the input value of the parameters

![image](https://github.com/Gutierre0x80/CSRF/assets/63872706/8a429857-8d76-498e-b007-6c2ee0959d9c)
