<div id="top"></div>
<!-- Project LOGO -->
<br />
<div align="center">
  
![RongIOC](https://socialify.git.ci/FFR66/RongIOC/image?description=1&descriptionEditable=Cyberspace%20Mapping%20APT%20Automated%20Line%20Extension%20Tool%20&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Fwww.wingby.cn%2Fimages%2Fteam_ico%2FFkalis.jpg&name=1&owner=1&pattern=Floating%20Cogs&pulls=1&stargazers=1&theme=Dark) 

  <h1 align="center">RongIOC</h1>
 
  **Cyberspace Mapping APT Automated Line Extension Tool**
  <br />
  **English | [中文](./README.md)**
  <br />
  <br />
  <a href="https://www.wingby.cn/">Team Website</a> 
  ·
  <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">Report a Bug</a>
  ·
  <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">Request a Feature</a> 
  ·
  <a href="#Contact-Author">Contact Author</a>
</p>
</div>

<!-- Table of Contents -->
<details>
  <summary><strong>Table of Contents</strong></summary>
  <ol>
    <li>
      <a href="#Precautions">Precautions</a>
    </li>
    <li>
      <a href="#About-This-Project">About This Project</a>
      <ul>
        <li><a href="#Build-Tools">Build Tools</a></li>
      </ul>
    </li>
    <li>
      <a href="#Getting-Started">Getting Started</a>
      <ul>
        <li><a href="#Dependencies">Dependencies</a></li>
        <li><a href="#Installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#Usage">Usage</a></li>
    <li><a href="#TODO">TODO</a></li>
    <li><a href="#Contributing">Contributing</a></li>
    <li><a href="#License">License</a></li>
    <li><a href="#Contact-Author">Contact Author</a></li>
    <li><a href="#Discussion-Group">Discussion Group</a></li>
    <li><a href="#Acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- About This Project -->
## Precautions
- **This project will call a large number of FOFA APIs, which may lead to exceeding the daily access limit. It is not recommended to use F points consumption!!**
- **This project will continue to be updated. There are still many unimplemented items in the TODO list, and it cannot meet all APT extension situations.**
- **This project is completely free and is only for learning purposes. Please do not use it for illegal destruction.**
- **This project is the public version of RongIOC.**

</br>

## About This Project

- **An automation tool for APT threat intelligence collection (APT network asset extension building).**
- **One of the Rong series tools (RongScan, RongFofa, RongHack, and other tools are not open-sourced and are used internally by the team. Contact the author for review if needed).**
- **Project Address: [https://github.com/WingBy-Fkalis/RongIOC](https://github.com/WingBy-Fkalis/RongIOC)** 
- **Project Team: WingBY Cybersecurity Team**
- **First Author: Fkalis**

![image](https://github.com/user-attachments/assets/d9e671fa-9218-4fe5-91c8-97ea76b4958b) 

When encountering various APT attacks, we not only need to defend against the current attack but also need to build more fingerprints based on the current sample, fingerprint, and other information, which is also known as extension. After trying a large number of open-source IOCs, the basic process is fixed. We attempt to automate it to reduce workload and improve efficiency.

For more details on the basic process, please refer to the figure below (from a training course given to a certain company).

</br>
![image](https://github.com/user-attachments/assets/7fcbdeaf-6b71-4031-9a9a-8220c6080d8b) 

<p align="right">(<a href="#top">Back to Top</a>)</p>



### Build Tools
You can directly use the packaged exe.

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Getting Started -->
## Getting Started

This is an example of how to build the project locally.
To get a local copy and set it up, you can follow the example steps below.

### Dependencies

* exe
  ```sh
  Directly use the packaged exe.
  ```

### Installation

_Below is an example of how to guide your audience on how to install and configure your application. This template does not require any external dependencies or services._

1. Clone the repository

   ```sh
   git clone https://github.com/WingBy-Fkalis/RongIOC.git 
   ```
2. Go to the RongIOC directory

   ```sh
   cd RongIOC
   ```
3. Run RongIOC.exe

   ```js
   RongIOC.exe -h
   ```

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Usage Example -->
## Usage
**1. Check for help**

   ```sh
   RongIOC.exe -h
   ```

   ```sh
  -h, --help            show this help message and exit
  -e EMAIL, --email EMAIL
                        fofa account
  -k KEY, --key KEY     fofa key
  -i IOC, --ioc IOC     basic ioc (syntax+time) (e.g.:(domain="neger.site" || domain="semain.tech" || domain="aliit.org") && before="2024-01-04"
  -f FILE, --file FILE  domain, ip's basic ioc file list (testing phase, may have bugs)
  -l LINE, --line LINE  the number of lines you want to get (default is 3)
  -n NUMBER, --number NUMBER
                        the maximum error of a single line (maximum asset quantity) (default is: 2500)
  -t THREAD, --thread THREAD
                        the number of concurrent threads (default is: 3)
   ```

![image](https://github.com/user-attachments/assets/250a4718-5e94-4df9-b507-767b4de73f17) 

**2. Quick extension**

   > -e Enter your fofa account
   > -k Enter your fofa key
   > -i Basic IOC syntax (recommend using domain+discovery time method (below))

   ```sh
   RongIOC.exe -e xxx -k xxx -i "(domain=\"neger.site\" || domain=\"semain.tech\") && before=\"2024-01-04\""
   ```

![image](https://github.com/user-attachments/assets/4d3d5f52-6863-4c7b-b0ea-f23a968c1267) 

**3. Automatic extension to obtain ioc**

![image](https://github.com/user-attachments/assets/c46915d9-5733-4da8-8993-bb11027aefd7) 

**4. Obtain extension information**

![image](https://github.com/user-attachments/assets/a6b430f6-467a-47f8-a50b-058e88a6c307) 

![image](https://github.com/user-attachments/assets/40d7d4b9-5f96-45bf-96ea-e0e9bc05e7b1) 

**5. Demonstration of automation results**
   ```sh
   RongIOC.exe -e xxx -k xxx -i "(domain=\"neger.site\" || domain=\"semain.tech\") && before=\"2024-01-04\""
   ```

> **Built extensions**
  ```sh
----------Number: 119-----------
base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ") &&
 server="nginx"
----------Number: 103-----------
cert.issuer.org="Let's Encrypt" && base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ")
----------Number: 102-----------
cert.issuer.cn="R3" && cert.issuer.org="Let's Encrypt" && base_protocol="tcp" && (banner=" 2023 " && banner=" GMT

Content-Type: text/html

Content-Length: 183

Connection: keep-alive" && banner=", 23 ")
----------{Empty string feature, can be added according to demand}------------
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

_Proceed to [Documentation](https://fkalis.cn/RongIOC) for more examples_

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Roadmap -->
## TODO

- [x] Support for FOFA Cyberspace Mapping
- [x] Optimize filtering and screening to improve speed
- [x] Use concurrent coroutines to improve speed
- [x] Support for empty field fingerprints
- [ ] Configuration file settings
- [ ] Further confirmation of suspicious targets
    - [ ] Use ThreatBook, Qax, and other platforms for confirmation
    - [ ] Automatically perform basic IOC path scanning
    - [ ] Body similarity comparison
    - [ ] Large model verification
- [x] Support for non-empty field fingerprints
- [ ] Support for OR conditions (e.g., the attack target often operates in multiple orgs, i.e., org:xxx || org:xxx)
- [ ] Optimize return results
- [ ] Automatically generate extension reports
- [ ] Support for a large number of fingerprint methods:
    - [x] ip
    - [x] port
    - [x] header
    - [x] cert
    - [x] asn
    - [x] os
    - [x] server
    - [x] jarm
    - [x] banner
    - [ ] body,ico (Unable to query information due to lack of FOFA commercial version, temporarily not compatible, will be added if an account is available)
    - [ ] body_hash
    - [ ] header_hash
    - [ ] js
    - [ ] js_md5
    - [ ] ....
- [ ] More cyberspace mapping engines
    - [x] FOFA
    - [ ] QUAKE
    - [ ] HUNTER
    - [ ] ZOOMEYE
    - [ ] ....
- [ ] ....

Proceed to the [open issues](https://github.com/WingBy-Fkalis/RongIOC/issues) page to view all requested features (as well as known issues).

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Contributing -->
## Contributing
One person's ideas are always limited. If you have any good suggestions or ideas, welcome to raise them in the issue, not necessarily code help, any contribution you make is **respected**.
You will gain access to the internal version, acknowledgment of open-source contributors.... Thank you for your support to this project!!

If you have any good suggestions, please fork this repository and create a pull request. You can also simply create an issue and add the label 'enhancement'. Don't forget to give the project a star! Thank you again!

1. Fork (Fork) this project
2. Create your Feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Create a Pull Request (Pull Request)

### Open Source Contributors List
<!-- readme: collaborators,contributors -start -->
<!-- readme: collaborators,contributors -end -->

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- License -->
## License

Distributed under the MIT License. See [LICENSE.txt](LICENSE.txt) for more information.


<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Contact Author -->
## Contact Author

#### Public Account: fkalis
<img width="1000" alt="1734073673283" src="https://github.com/user-attachments/assets/affaa351-bde5-4c82-815b-71b252568f17; /> 

#### WeChat: WingBy_fkalis (Please note the purpose)
![image](https://github.com/user-attachments/assets/00fdb3fb-2497-48de-ae59-5a3508526cb3) 

#### Team: WingBy Cybersecurity Team (https://www.wingby.cn/) 

<p align="right">(<a href="#top">Back to Top</a>)</p>


## Discussion Group
If the QR code is invalid, you can add the author to join the group
</br>
<img width="350" alt="1734272402262" src="https://github.com/user-attachments/assets/6819981a-8d8b-47be-ba84-c3afe98ec14e; />



<!-- Acknowledgments -->
## Acknowledgments

List the resources you find helpful here, and give thanks. I have added some of my favorite resources so you can get started quickly!

* [FOFA Asset Extension Practical Series: Sidewinder APT Organization](https://mp.weixin.qq.com/s/r8VLB4aWTFScGXwyOjTpVQ) 
* [FOFA Asset Extension Practical Series: APT-C-23 Android Terminal](https://mp.weixin.qq.com/s/ODv4d8PKoBAAaCF5Cn_GcA)(To be implemented) 
* [FOFA Asset Extension Practical Series: Ducktail Criminal Organization](https://mp.weixin.qq.com/s/NrUbuSIjA8qwYMw9zVFscw) 
* [Using FOFA for a Practical APT Bitter Tracking](https://mp.weixin.qq.com/s/dhuh3xRCllR2uevNxT1r7Q) 
* [Public Sample Project](https://github.com/stamparm/maltrail/blob/master/trails/static/malware) 
* [FOFA](https://fofa.info/) 
* [ThreatBook Intelligence Center](https://x.threatbook.com/) 


<p align="right">(<a href="#top">Back to Top</a>)</p>


