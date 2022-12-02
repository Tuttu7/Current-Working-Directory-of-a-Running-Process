#### Find the Current Working Directory of a Running Process


```
[tuttu@fedora test]$ lsof -p 4982 | grep cwd
brave-bro 4982 tuttu  cwd    DIR   0,37     2348     257 /home/tuttu
```


#### Use the pwdx command to identify the current working directory of the process :

```
[tuttu@fedora test]$ pwdx 4982
4982: /home/tuttu
```

#### Note that the pwdx command doesn’t display where the process was invoked. It just shows where it currently runs from.


#### The lsof (list open files) command returns information about all processes that are currently active. We can get a lot of information about processes with this command. 

```
[tuttu@fedora test]$ lsof -p 4982 | grep cwd
brave-bro 4982 tuttu  cwd    DIR   0,37     2348     257 /home/tuttu
```
