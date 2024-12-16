<div id="top"></div>
<!-- 项目 LOGO -->
<br />
<div align="center">
  
![RongIOC](https://socialify.git.ci/FFR66/RongIOC/image?description=1&descriptionEditable=%E7%BD%91%E7%BB%9C%E7%A9%BA%E9%97%B4%E6%B5%8B%E7%BB%98APT%E8%87%AA%E5%8A%A8%E5%8C%96%E6%8B%93%E7%BA%BF%E5%B7%A5%E5%85%B7%20%0A(Cyberspace%20Mapping%20APT%20Automated%20Line%20Extension%20Tool%20)&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Fwww.wingby.cn%2Fimages%2Fteam_ico%2FFkalis.jpg&name=1&owner=1&pattern=Floating%20Cogs&pulls=1&stargazers=1&theme=Dark)

  <h1 align="center">RongIOC</h1>
  
  **网络空间测绘APT自动化拓线工具**
  <br />
  **(Cyberspace Mapping APT Automated Line Extension Tool )**
  <p align="center">
    <a href="./README.md"><strong>浏览文档 »</strong></a>
    
  **中文** | [English](./README.en.md)
    <br />
    <br />
    <a href="https://www.wingby.cn/">团队官网</a>
    ·
    <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">反馈 Bug</a>
    ·
    <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">请求新功能</a>
    ·
    <a href="#联系作者">联系作者</a>
  </p>
</div>

<!-- 目录 -->
<details>
  <summary><strong>目录</strong></summary>
  <ol>
    <li>
      <a href="#注意事项">注意事项</a>
    </li>
    <li>
      <a href="#关于本项目">关于本项目</a>
      <ul>
        <li><a href="#构建工具">构建工具</a></li>
      </ul>
    </li>
    <li>
      <a href="#开始">开始</a>
      <ul>
        <li><a href="#依赖">依赖</a></li>
        <li><a href="#安装">安装</a></li>
      </ul>
    </li>
    <li><a href="#使用方法">使用方法</a></li>
    <li><a href="#TODO">TODO</a></li>
    <li><a href="#贡献">贡献</a></li>
    <li><a href="#许可证">许可证</a></li>
    <li><a href="#联系作者">联系作者</a></li>
    <li><a href="#交流群">交流群</a></li>
    <li><a href="#致谢">致谢</a></li>
  </ol>
</details>



<!-- 关于本项目 -->
## 注意事项
- **本项目会调用大量的FOFA接口,可能会导致当日访问次数超过的情况,不建议开启F点消耗使用！！**
- **本项目将持续更新，目前TODO中还有很多没有更新，并不能满足全部的APT拓线情况**
- **本项目完全免费，仅作为学习使用，请不要进行非法破坏**
- **本项目为RongIOC的公开版本**

</br>

## 关于本项目

- **一款用于APT威胁情报收集(APT网络资产拓线构建)的自动化工具**
- **Rong系列工具之一(RongScan,RongFofa,RongHack等工具暂不开源,团队内部使用,有需要联系作者审核)**
- **项目地址: [https://github.com/WingBy-Fkalis/RongIOC](https://github.com/WingBy-Fkalis/RongIOC)**
- **项目所属团队: WingBY网络安全团队**
- **第一作者: Fkalis**
  
![image](https://github.com/user-attachments/assets/d9e671fa-9218-4fe5-91c8-97ea76b4958b)


在遇到各种APT攻击的时候，我们不仅需要进行防御当前的攻击，也需要基于当前的样本,指纹,等信息去构建更多的指纹，也就是所说的拓线，在进行了大量开源IOC的尝试其基本流程是固定的
尝试将其进行自动化，减少工作量，提升效率

基本流程参考下图（在给某公司进行APT培训的时候的课件）
</br>
![image](https://github.com/user-attachments/assets/7fcbdeaf-6b71-4031-9a9a-8220c6080d8b)


<p align="right">(<a href="#top">返回顶部</a>)</p>



### 构建工具
直接使用打包好的exe即可

<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 开始 -->
## 开始

这是一份在本地构建项目的指导的例子。
要获取本地副本并且配置运行，你可以按照下面的示例步骤操作。

### 依赖

* exe
  ```sh
  直接使用打包好的exe即可
  ```

### 安装

_下面是一个指导你的受众如何安装和配置你的应用的例子。这个模板不需要任何外部依赖或服务。_

1. 克隆本仓库

   ```sh
   git clone https://github.com/WingBy-Fkalis/RongIOC.git
   ```
2. 来到RongIOC目录

   ```sh
   cd RongIOC
   ```
3. 运行RongIOC.exe

   ```js
   RongIOC.exe -h
   ```

<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 使用方法 示例 -->
## 使用方法
  **1. 查看帮助**

   ```sh
   RongIOC.exe -h
   ```

   ```sh
  -h, --help            show this help message and exit
  -e EMAIL, --email EMAIL
                        fofa账号
  -k KEY, --key KEY     fofa密钥
  -i IOC, --ioc IOC     基础ioc (语法+时间) (例如:(domain="neger.site" || domain="semain.tech" || domain="aliit.org") && before="2024-01-04"
  -f FILE, --file FILE  域名,ip的基础ioc文件列表 (测试阶段,可能有bug)
  -l LINE, --line LINE  想要获取的拓线数量 (默认为3)
  -n NUMBER, --number NUMBER
                        单条拓线的最大误差(最大资产量) (默认为:2500)
  -t THREAD, --thread THREAD
                        并发线程数 (默认为:3)
   ```


![image](https://github.com/user-attachments/assets/250a4718-5e94-4df9-b507-767b4de73f17)

  **2. 快速进行拓线**

   > -e 输入fofa的账户
   > -k 输入fofa的密钥
   > -i 基础IOC语法 (推荐使用 域名+发现时间的方式(如下))

   ```sh
   RongIOC.exe -e xxx -k xxx -i "(domain=\"neger.site\" || domain=\"semain.tech\") && before=\"2024-01-04\""
   ```

![image](https://github.com/user-attachments/assets/4d3d5f52-6863-4c7b-b0ea-f23a968c1267)


  **3. 自动拓线获取ioc**

![image](https://github.com/user-attachments/assets/c46915d9-5733-4da8-8993-bb11027aefd7)


  **4. 获取拓线信息**

![image](https://github.com/user-attachments/assets/a6b430f6-467a-47f8-a50b-058e88a6c307)

![image](https://github.com/user-attachments/assets/40d7d4b9-5f96-45bf-96ea-e0e9bc05e7b1)



  **5. 自动化成果展示**
   ```sh
   RongIOC.exe -e xxx -k xxx -i "(domain=\"neger.site\" || domain=\"semain.tech\") && before=\"2024-01-04\""
   ```

> **构建的拓线**
  ```sh
----------数量: 119-----------
base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ") && server="nginx"
----------数量: 103-----------
cert.issuer.org="Let's Encrypt" && base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ")
----------数量: 102-----------
cert.issuer.cn="R3" && cert.issuer.org="Let's Encrypt" && base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ")
----------{空字符串特征,可根据需求添加}------------
os="" && icp="" && cert.subject.org="" && cname=""
   ```

<img width="1280" alt="8d1be1711049c93b0e4f391e2757a8e" src="https://github.com/user-attachments/assets/c3d03e40-bdbe-429f-9049-69d19092a1f3" />

![0a4987f484384188a7b8551452f198b](https://github.com/user-attachments/assets/11f78cda-1b36-4b1a-8da0-1ab1771bff5b)

![819130c58912f9a5cc6e3db87c82b6a](https://github.com/user-attachments/assets/8ba4125f-e4ae-48c7-a975-5e7aff81e896)

![784635cdab75373d0ed7461134bb7e6](https://github.com/user-attachments/assets/c36f8015-88ba-4980-9f69-bbc6f8573866)

![d26992ebafff3d611b00a79a0a4fcd1](https://github.com/user-attachments/assets/5675185a-d800-4898-bb89-94bbf9028c66)

![b98f69f2ce3d5a63b16da66ce0135cb](https://github.com/user-attachments/assets/854dce89-d805-414b-9367-5e5463bf4654)

![e3b3cd10b981b2e398c52fc45f15661](https://github.com/user-attachments/assets/6b8636d0-c241-4c25-85e5-9547384ff3b5)

![26843b348fd5e4b1901ee98bd8a8ffd](https://github.com/user-attachments/assets/f1901e3d-0a79-423c-af4a-456e7753d869)

</br>

_转到 [文档](https://github.com/WingBy-Fkalis/RongIOC) 查看更多示例_

<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 路线图 -->
## TODO

- [x] 支持FOFA网络空间测绘
- [x] 优化过滤筛选,提高速度
- [x] 使用并发协程,提高速度
- [x] 支持空字段指纹
- [ ] 配置文件设置
- [ ] 进一步确认可疑目标
    - [ ] 使用微步,qax等平台进行确认
    - [ ] 自动进行基础IOC路径扫描
    - [ ] body相似度比较
    - [ ] 大模型验证
- [x] 支持非空字段指纹
- [ ] 支持或条件(例如:攻击目标经常在多个org中进行，即org:xxx || org:xxx)
- [ ] 优化返回结果
- [ ] 自动生成拓线报告
- [ ] 支持大量的指纹方式:
    - [x] ip
    - [x] port
    - [x] header
    - [x] cert
    - [x] asn
    - [x] os
    - [x] server
    - [x] jarm
    - [x] banner 
    - [ ] body,ico (由于没有FOFA商业版,无法查询到其信息,暂时无法兼容,如果有机会有账户的话,会进行添加)
    - [ ] body_hash
    - [ ] header_hash
    - [ ] js
    - [ ] js_md5
    - [ ] ....
- [ ] 更多的网络空间测绘引擎
    - [x] FOFA
    - [ ] QUAKE
    - [ ] HUNTER
    - [ ] ZOOMEYE
    - [ ] ....
- [ ] .......

到 [open issues](https://github.com/WingBy-Fkalis/RongIOC/issues) 页查看所有请求的功能 （以及已知的问题）。

<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 贡献 -->
## 贡献
一个人的思路终归是有限的，如果有你有什么好的建议，好的思路，欢迎在issue提出，不一定是代码上的帮助，你所做出的任何贡献都是**受人尊敬**的。
您将获得内部版本的使用权限，开源贡献者的致谢....感谢您对本项目的支持！！

如果你有好的建议，请复刻（fork）本仓库并且创建一个拉取请求（pull request）。你也可以简单地创建一个议题（issue），并且添加标签「enhancement」。不要忘记给项目点一个 star！再次感谢！

1. 复刻（Fork）本项目
2. 创建你的 Feature 分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的变更 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到该分支 (`git push origin feature/AmazingFeature`)
5. 创建一个拉取请求（Pull Request）

### 开源贡献者列表
<!-- readme: collaborators,contributors -start -->
<!-- readme: collaborators,contributors -end -->

<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 许可证 -->
## 许可证

根据 MIT 许可证分发。打开 [LICENSE.txt](LICENSE.txt) 查看更多内容。


<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 联系作者 -->
## 联系作者

#### 公众号：fkalis
<img width="1000" alt="1734073673283" src="https://github.com/user-attachments/assets/affaa351-bde5-4c82-815b-71b252568f17" />

#### 微信号: WingBy_fkalis（备注来意）
![image](https://github.com/user-attachments/assets/00fdb3fb-2497-48de-ae59-5a3508526cb3)




#### 所属团队：WingBy网络安全团队 (https://www.wingby.cn/)


<p align="right">(<a href="#top">返回顶部</a>)</p>


## 项目交流群
如果二维码失效可以添加作者加群
</br>
<img width="350" alt="1734272402262" src="https://github.com/user-attachments/assets/6819981a-8d8b-47be-ba84-c3afe98ec14e" />



<!-- 致谢 -->
## 致谢

在这里列出你觉得有用的资源，并以此致谢。我已经添加了一些我喜欢的资源，以便你可以快速开始！

* [FOFA资产拓线实战系列：响尾蛇APT组织](https://mp.weixin.qq.com/s/r8VLB4aWTFScGXwyOjTpVQ)
* [FOFA资产拓线实战系列：APT-C-23 Android端](https://mp.weixin.qq.com/s/ODv4d8PKoBAAaCF5Cn_GcA)(待实现)
* [FOFA资产拓线实战系列：Ducktail犯罪组织](https://mp.weixin.qq.com/s/NrUbuSIjA8qwYMw9zVFscw)
* [用FOFA进行一场APT Bitter追踪的实战](https://mp.weixin.qq.com/s/dhuh3xRCllR2uevNxT1r7Q)
* [公开样本项目](https://github.com/stamparm/maltrail/blob/master/trails/static/malware)
* [FOFA](https://fofa.info/)
* [微步情报中心](https://x.threatbook.com/)

<p align="right">(<a href="#top">返回顶部</a>)</p>



