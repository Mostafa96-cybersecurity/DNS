# 1- What is DNS ?
***it's shortcut of Domain Name System***

*it provides a simple way to communicate with devices on the internet without remember the ip address .*

*See The Photo Below*

![DNS](https://user-images.githubusercontent.com/84593266/138587993-5d4f1790-398d-43a7-a17f-7bc70b362cf3.png)

*You wnat to browse `https://www.google.com` you wrire `google.com` then press Enter then the site will open it's easy for you but the
process that you can not see is*
```
1- You go To The DNS Server 
2- Then The DNS reply with the ip address of google to you Then You Go to google
this is simple express
```

*after this process the IP Address of google stored in your DNS Cache try to write in your cmd `ipconfig /displaydns` you will get the DNS cache*

**Simple Scenario**

*mike wants to visit`Facebook.com`site 
he opened his browser and write `facebook.com`
The Facebook has responded to his Answer.
how does this process Work ?
when mike wrote facebook.com and pressed Enter
He asked The DNS First >>> What is the IP Address of Facebook.com ?
The DNS Responded To his Answer The IP Address is `102.132.97.35` 
Then Mike Take The IP and connect to Facebook
This process in First Time Mike visit The Facebook
Mike Stored The IP Address in his DNS cache 
in Second Time Mike Will go To DNS Cache to check To Get The IP Address He Will Not Go Far Again To Ask For The IP Address of Facebook*

*This is Simple express about How DNS works in Your Local PC*

# 2- DNS Hierarchy 
```
1- Root Domain
2- Top-Level-Domains (TLD)
3- Second-Level-Domaines (SLD)
```
*we will Look in DNS in Simple deep we now know how DNS Works in out Computer now lets know about DNS in deep ` DNS Hierarchy`*

*it's so easy i will make it very simple do not worry.*

<img width="653" alt="img-1" src="https://user-images.githubusercontent.com/84593266/138589849-c1c134f6-ede0-4621-b2fb-b1a44e78a708.png">

*1- First level (Root) we can say it Root Hint it have all The Domains of DNS*

*2- TOP Level Domain (TLD) i will try to make it very easy. we have*
```
facebook.com
google.com
rasmussen.edu
NASA.gov
Army.mil
```
*Simply Look at The Photo Below You Will know What i Mean*

![what-is-a-domain-name](https://user-images.githubusercontent.com/84593266/138590066-5116688d-d0af-4b6b-a383-de10c5c99d4c.png)

*we will get a website and analysis it Then every point Will be clear To You*
`https://www.en.wikiversity.org/wiki/Computer_Networks`
*we will analysis it step by step we all know `https` it's cert for security*
```
www : it's (world wide web)
en. : This is subdomain 
wikiversity. : This is The Domain or Second-Level-Domain (SLD) 
edu : it's TOP-Level-Domain (TLD)
/wiki/Computer_Networks : it's subdirectory in the web server 
```
*i think it's clear know Look at the photo again*

# 3- DNS Record

*DNS is not for websites only we have DNS record DNS record Types*
```
1- A Record : to Resolve IPv4 Address such as 174.16.156.15
2- AAAA Record : To Resolve IPv6 Address such as 2606:4700:20::681a:be5 
3- CNAME Record : This Record For Another Domain such as we have site have online shop (shop.store.net)
it has a Record like shop.shopify.net simply it has record in server named shopify.net with name shop `shop.shopify.net`
4- MX Record : This kind of Record Resolve The Address of Servers That Have email server for The domain `Facebook.com` Has MX Record (smtpin.vvv.facebook.com) to handle any email.
5- TXT Record : This Record handle any text data stored as .TXT 
i thinkg it's simple
```
# 4- Summary

**DNS Request**

*1- You ask For The IP address of any website You Want TO visit such as `github.com`

*2- check your local DNS Cache if The IP Adderss in The DNS Cach if it's in you will redirect to the website if not let's go to the next step 

*3- You Will ask Your ISP DNS this DNS You Can change it to any DNS such as `8.8.8.8 or 8.8.4.4` if the DNS has The IP Address of `github.com` it will get it back to you with the IP Adderss if not . 

*4- your request will be forwarded to The DNS Root Hint This is The Backbone of All DNS Servers it has ALL (TLD) it will look to your request 
(github.com) he will redirect your request to the .com (TLD) to get the IP Address then the request will go back to you with the IP Address Then your DNS cache Will store This with (TTL) in second if .
**That's it some useful command about DNS** 

ipconfig /displaydns : to see the DNS Cache and TTL

ipconfig /flushdns

dnslookup : To get information about domain `nslookup google.com`

there is websites you can use such as 

[MXTOOLBOX](https://mxtoolbox.com/).

[dnslookup](https://dnslookup.online/). it can check for the Type of Record

# Scorpion@oPs




