
* Caller ID - https://calleridtest.com/
* Jenny AI - An AI auto-writing tool that automatically writes your essays and emails for you. All you have to do is give it a title and a couple of sentences: https://jenni.ai/
* Quillbot- A paraphrasing website that rewrites everything as plagiarism free text. Super handy if you're in college: https://quillbot.com/
* This website lets you convert files to any format you want for free: https://convertio.co/

* * * 

### Send Anonymous Text Messages (Only one a day Free)

``` sudo git clone https://github.com/machine1337/fake-sms ```

``` cd fake-sms ```

``` sudo chmod 755 run.sh  ```

``` sudo ./run.sh ```

* When we open "Fake-SMS" Repo, we can see it is a simple BASH script. When we scroll down to lines 119-120, we can see a curl command to textbelt.com. Apparently, this script simply uses this SMS site to send text messages.

Use the curl command to send SMS: 

* First, we need to open an account at textbelt.com. When we open an account, we can send one fake SMS message per day or we can purchase credits and get an API key to use their service.

* Once you have an API from your account we can generate our own text messages without the Fake-SMS script directly by creating a curl command in Linux 

``` curl -X POST https://textbelt.com/text --data-urlencode phone='<ENTER FULL PHONE NUMER>' --data-urlencode= message='<ENTER MESSAGE>' -d key=<YOU API KEY> ```

* This service responds with a message detailing the success of sending my message and the number of messages left in my quota.

[SOURCE](https://www.hackers-arise.com/post/social-engineering-attacks-creating-a-fake-sms-message)
