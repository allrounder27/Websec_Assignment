# Websec_Assignment
## Problem 1 -

https://backdoor.sdslabs.co/challenges/BRWSR

### Solution -

Open Develop tools. Then go to Network conditions and change the user agent to custom i.e, SDSLabs and refresh.

### Flag -

Welcome!! Thanks for using our browser! Here's a flag for you: e77aec24943bb31c63547812d1130c67d0e7e941bf5d85bfef0492cc68050aef

## Problem 2 -

https://backdoor.sdslabs.co/challenges/WHAT-IP

### Solution -

In this problem the hint is that it only allows the ip 127.0.0.1. So we copy the curl and use X-Forwarded-For, and use the command-
  
```$ curl -H 'X-Forwarded-For: 127.0.0.1' 'http://hack.bckdr.iindex.php' -H 'Connection: keep-alive' -H 'Cache-Control: max-age=0' -H 'Upgrade-Insecure-Requests: 1' -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.106 Safari/537.36' -H 'Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9' -H 'Accept-Language: en-US,en;q=0.9' --compressed --insecure```

### Flag -

Access granted. Flag is d025c4ca8e71501df3581d995c9d838801125d16b0468f6b980969d4

## Problem 3 -

https://2019shell1.picoctf.com/problem/12284/

### Solution -

We are able to login without giving any id or password. So it seems to check the password only for admins. Therefore we need to check the cookies (I used EditThisCookie chrome extension) in which we see that admin is set to false, just change it to true.

### Flag - 

Flag: picoCTF{th3_c0nsp1r4cy_l1v3s_6f2c20e9}

## Problem 4 -

https://2019shell1.picoctf.com/problem/12255/

### Solution - 

This one is same as the first one just change the user agent to picobrowser as before.

### Flag - 

picoCTF{p1c0_s3cr3t_ag3nt_bbe8a517}



