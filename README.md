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
    <a href="https://github.com/WingBy-Fkalis/RongIOC/README.md"><strong>浏览文档 »</strong></a>
    
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
    <li><a href="#致谢">致谢</a></li>
  </ol>
</details>



<!-- 关于本项目 -->
## 关于本项目

- **一款用于APT威胁情报收集(APT网络资产拓线构建)的自动化工具**
- **Rong系列工具之一(RongScan,RongFofa,RongHack等工具暂不开源,团队内部使用,有需要联系作者审核)**
- **项目地址: [https://github.com/WingBy-Fkalis/RongIOC](https://github.com/WingBy-Fkalis/RongIOC)**
- **项目所属团队: WingBY网络安全团队**
- **第一作者: Fkalis**
  
![image](https://github.com/user-attachments/assets/650b3c6d-379f-4fa8-9c59-526d279bacf8)

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

_转到 [文档](https://example.com) 查看更多示例_

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

贡献让开源社区成为了一个非常适合学习、启发和创新的地方。你所做出的任何贡献都是**受人尊敬**的。

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
<img width="855" alt="1734073673283" src="https://github.com/user-attachments/assets/affaa351-bde5-4c82-815b-71b252568f17" />

#### 微信号: WingBy_fkalis（备注来意）
![image](https://github.com/user-attachments/assets/00fdb3fb-2497-48de-ae59-5a3508526cb3)




#### 所属团队：WingBy网络安全 (https://www.wingby.cn/)


<p align="right">(<a href="#top">返回顶部</a>)</p>



<!-- 致谢 -->
## 致谢

在这里列出你觉得有用的资源，并以此致谢。我已经添加了一些我喜欢的资源，以便你可以快速开始！

* [FOFA资产拓线实战系列：响尾蛇APT组织](https://mp.weixin.qq.com/s/r8VLB4aWTFScGXwyOjTpVQ)

<p align="right">(<a href="#top">返回顶部</a>)</p>



