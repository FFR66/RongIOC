
<div id="top"></div>
<!-- Project LOGO -->
<br />
<div align="center">
  
![RongIOC](https://socialify.git.ci/FFR66/RongIOC/image?description=1&descriptionEditable=Cyberspace%20Mapping%20APT%20Automated%20Line%20Extension%20Tool&font=Inter&forks=1&issues=1&language=1&logo=https%3A%2F%2Fwww.wingby.cn%2Fimages%2Fteam_ico%2FFkalis.jpg&name=1&owner=1&pattern=Floating%20Cogs&pulls=1&stargazers=1&theme=Dark) 

  <h1 align="center">RongIOC</h1>
  
  **Cyberspace Mapping APT Automated Line Extension Tool**
  <br />
  <p align="center">
    <a href="https://github.com/WingBy-Fkalis/RongIOC/README.md"><strong>View Documentation »</strong></a>
    
  Chinese | [English](./README.en.md)
    <br />
    <br />
    <a href="https://www.wingby.cn/">Team Website</a> 
    ·
    <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">Report a Bug</a>
    ·
    <a href="https://github.com/WingBy-Fkalis/RongIOC/issues">Request a Feature</a> 
    ·
    <a href="#contact-author">Contact Author</a>
  </p>
</div>

<!-- Table of Contents -->
<details>
  <summary><strong>Table of Contents</strong></summary>
  <ol>
    <li>
      <a href="#about-the-project">About the Project</a>
      <ul>
        <li><a href="#building-tools">Building Tools</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#todo">TODO</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact-author">Contact Author</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- About the Project -->
## About the Project

- **An automated tool for APT threat intelligence collection (APT network asset line construction)**
- **One of the Rong series tools (RongScan, RongFofa, RongHack, etc., are not open-sourced and are used internally by the team. Contact the author for access review)**
- **Project Address: [https://github.com/WingBy-Fkalis/RongIOC](https://github.com/WingBy-Fkalis/RongIOC)** 
- **Project Team: WingBY Cybersecurity Team**
- **First Author: Fkalis**

When encountering various APT attacks, we not only need to defend against the current attack but also need to construct more fingerprints based on the current sample, fingerprint, and other information, which is also known as line extension. After trying a large number of open-source IOCs, the basic process is fixed. We attempt to automate it to reduce workload and improve efficiency.

Refer to the following diagram for the basic process (from a training course given to a company).

</br>

![image](https://github.com/user-attachments/assets/7fcbdeaf-6b71-4031-9a9a-8220c6080d8b) 


<p align="right">(<a href="#top">Back to Top</a>)</p>



### Building Tools
You can use the pre-packaged exe directly.

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Getting Started -->
## Getting Started

This is an example of how to build the project locally.
To get a local copy and set it up, you can follow these example steps.

### Prerequisites

* exe
  ```sh
  Use the pre-packaged exe directly.
  ```

### Installation

_Below is an example of how to install and configure your application. This template does not require any external dependencies or services._

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



<!-- Usage Examples -->
## Usage

_Refer to [Documentation](https://example.com) for more examples_

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Roadmap -->
## TODO

- [x] Support FOFA Cyberspace Mapping
- [x] Optimize filtering and screening to improve speed
- [x] Use concurrent coroutines to improve speed
- [x] Support empty field fingerprints
- [ ] Configuration file settings
- [ ] Further confirm suspicious targets
    - [ ] Use platforms such as ThreatBook, Qax for confirmation
    - [ ] Automatically perform basic IOC path scanning
    - [ ] Body similarity comparison
    - [ ] Large model verification
- [ ] Support a variety of fingerprint methods:
    - [x] ip
    - [x] port
    - [x] header
    - [x] cert
    - [x] asn
    - [x] os
    - [x] server
    - [x] jarm
    - [x] banner 
    - [ ] body,ico (Due to lack of FOFA commercial version, unable to query its information, temporarily not compatible, if there is an opportunity to have an account, it will be added)
    - [ ] ....
- [ ] More cyberspace mapping engines
    - [x] FOFA
    - [ ] QUAKE
    - [ ] HUNTER
    - [ ] ZOOMEYE
    - [ ] ....
- [ ] .......

Check out the [open issues](https://github.com/WingBy-Fkalis/RongIOC/issues) page to see all requested features (and known issues).

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Contributing -->
## Contributing

Contributions make the open-source community a great place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a good suggestion, please fork the project and create a pull request. You can also simply open an issue and add the 'enhancement' label. Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Collaborators & Contributors
<!-- readme: collaborators,contributors -start -->
<!-- readme: collaborators,contributors -end -->

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- License -->
## License

Distributed under the MIT License. See [LICENSE.txt](LICENSE.txt) for more information.


<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Contact the Author -->
## Contact Author

#### WeChat Official Account: fkalis
<img width="855" alt="1734073673283" src="https://github.com/user-attachments/assets/affaa351-bde5-4c82-815b-71b252568f17" />

#### WeChat ID: WingBy_fkalis (Please indicate your purpose)
![image](https://github.com/user-attachments/assets/00fdb3fb-2497-48de-ae59-5a3508526cb3) 

#### Team: WingBy Cybersecurity Team (https://www.wingby.cn/) 

<p align="right">(<a href="#top">Back to Top</a>)</p>



<!-- Acknowledgments -->
## Acknowledgments

List any resources you find helpful and give credit here. I have added some of my favorite resources to get you started quickly!

* [FOFA Asset Extension Series: Rattlesnake APT Organization](https://mp.weixin.qq.com/s/r8VLB4aWTFScGXwyOjTpVQ)
