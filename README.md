# vibeWaf 
* 使用方法
~~~bash
python3 ./identYwaf.py 

Usage: python identYwaf.py [options] <host|url>

Options:
  --version           Show program's version number and exit
  -h, --help          Show this help message and exit
  --delay=DELAY       测试之间的延迟(秒) (默认: 0)
  --timeout=TIMEOUT   响应超时(秒) (默认: 10)
  --proxy=PROXY       HTTP代理地址 (e.g. "http://127.0.0.1:8080")
  --proxy-file=PRO..  从文件中加载(s)HTTP代理列表
  --random-agent      使用随机的HTTP User-Agent 请求头
  --code=CODE         被拒绝响应中预期的HTTP代码
  --string=STRING     被拒绝响应中的预期字符串
  --post              使用POST主体发送有效负载
~~~
* 可以使用 proxychains4 代理流量
~~~bash
proxychains4 ./vibeWaf  'http://www.baidu.com'
~~~
