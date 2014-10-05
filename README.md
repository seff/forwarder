本项目移植于[Forwarder](https://github.com/cdhigh/Forwarder)，运行在REDHAT的OPENSHIFT之上，因为OPENSHIFT完全免费，所以每个人都可以自己进行搭建，不用再分享原作者在AppFog上的流量。具体介绍请参考原项目说明文件，OPENSHIFT的具体使用方式请GOOGLE之。

**用法**：

>http://hostedurl?u=url&k=AUTHKEY&t=timeout

>**解析**：

>hostedurl: 你搭建的转发服务器的URL

>url: 需要转发到url，需要先使用urllib.quote转义，特别是如果有&符号

>AUTHKEY: 为了防止滥用，需要提供一个key，为ALLOW_KEYS里面的任何一个值

>timeout: [可选]超时时间，默认为30s

例子请参照KindleEar项目的books/ZhihuDaily.py (知乎日报)
