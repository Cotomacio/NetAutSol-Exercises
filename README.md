# NetAutSol-Exercises
### Hands-on exercises proposed on Building Network Automation Solutions by (@ipspace)

## 1. GETTING STARTED: BUILD THE LAB
- **Selecting the gear:** 
  - I decided to use Cisco VIRL in my lab for two reasons:
    1. I am comfortable with the syntax
    2. It's portable
  - The drawback is that it took me a while to setup and figure out how to use it, but the VIRL [book](https://www.amazon.com/VIRL-BOOK-Step-Step-Internet-ebook/dp/B01M0N517P) helped me a lot.
  
- **Building the lab:**
  - I used @ipspace [bash script](https://github.com/ipspace/NetOpsWorkshop/blob/master/install/install.sh) to be Up and Running very quick on my VM with Ubuntu 16.04 LTS
  - In order to have a recover point after major changes on my environment I decided not use another technology (Vagrant) but VM Fusion features like Clone and Snapshot

- **Set up Git and Github**
  - This is no brainer: After creating my account on Github I installed *Git* on my Ubuntu VM with **sudo apt-get -qq install git**
  
- **Publish a file on Github**  
  - Topology: I have 3x routers running IOSv with basic IP addressing and OSPF 1 Area 0 configured using AutoNetkit
  
     ![My Topology](https://github.com/Cotomacio/NetAutSol-Exercises/blob/master/1-getting-started-topo.png)

     - I have collected `show ip ospf neighbor` using Ansible Raw module and published here using a pull request
