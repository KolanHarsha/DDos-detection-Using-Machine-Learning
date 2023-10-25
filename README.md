# DDos-detection-Using-Machine-Learning
## **What is DDOs(Distributed denial of service)?**
A Distributed Denial of Service (DDoS) attack is a malicious attempt to disrupt the regular functioning of a network, service, website, or online resource by overwhelming it with a flood of internet traffic. In a DDoS attack, multiple compromised computers or devices (often referred to as "botnets") are coordinated to send an excessive volume of data requests or traffic to the target, making it difficult or impossible for legitimate users to access the targeted resource. A ddos attack usually occurs in layer-7(Application-layer),layer-4(Transport-layer) and layer-3(Network-layer) of the Networking model. In this work we try to detect a DDos attack in the layer-7 using machine-learning algorithms(Random-forests and Gradient-Boosting).
## **What is a Botnet**
A botnet is a network of compromised computers or devices controlled by a single entity, often a cybercriminal or hacker, without the owners' knowledge. These compromised devices, referred to as "bots" or "zombies," can be infected with malware, allowing the attacker to commandeer them remotely.
In DDoS attacks, botnets are used to amplify and distribute attack traffic. The attacker instructs the bots to simultaneously send a flood of requests to the target, overwhelming its resources. Since botnets can consist of thousands or even millions of devices, they generate a massive volume of traffic, making it difficult for the target to distinguish legitimate requests from the malicious ones.
## **Different types of DDos attacks in layer-7**
### **Slowloris attack**
A Slowloris attack is a type of DDoS attack that targets web servers. It works by opening multiple connections to the server and sending partial HTTP requests, keeping them open by sending data very slowly. This ties up server resources, preventing new connections and legitimate requests. Slowloris doesn't require a large number of attacking machines, making it hard to detect. It focuses on resource exhaustion, causing the server to become slow or unresponsive.
### **HTTP GET/POST flood attack**
An HTTP GET/POST flood attack is a type of DDoS attack that targets web servers. Attackers send a massive number of GET or POST requests to overwhelm the server's capacity. GET requests retrieve data, while POST requests send data to the server, both tying up server resources. This flood of requests can slow down or crash the server, making the targeted website or application inaccessible. 
## **Dataset description**
The dataset has two sets balanced dataset and imbalanced dataset both with 84 features. The balanced dataset has 50% benign flows and 50% Ddos flows. The main goal of this work is to detect ddos attacks in application layers in which the  attack traffic is in smaller proportion when compared to benign flows hence imbalnced dataset is used which has 83% benign flows and 17% Ddos flows. The total number of benign flows in imbalnced dataset are 6321980 and total number of Ddos flows in the imbalanced dataset are 1294529.
## **<img width="291" alt="Screenshot 2023-10-09 215033" src="https://github.com/KolanHarsha/DDos-detection-Using-Machine-Learning/assets/110462466/1161405f-2586-4911-ab09-be2f82675f6b">**
## **Tools**
<img src="https://github.com/KolanHarsha/DDos-detection-Using-Machine-Learning/assets/110462466/88e29b73-06a2-48ac-8e80-0cd755dd980e" alt="jup" width="150" height="100">
<img src="https://github.com/KolanHarsha/DDos-detection-Using-Machine-Learning/assets/110462466/91408e94-709a-4639-b3ce-72995848c519" alt="azure" width="175" height="100">

## **How to run the Notebook**
### **Install Neccessary packages**
Ip-Address:
```bash
pip install ipaddress
 ```
Numpy:
```bash
pip install numpy
 ```
Pandas:
```bash
pip install pandas
 ```
Matplotlib:
```bash
pip install matplotlib
 ```
Seaborn:
```bash
pip install seaborn
 ```
Scikit-learn:
```bash
pip install scikit-learn
 ```
### **Running on Azure Cloud Platform**
1. Go to the [Azure Machine Learning ](https://azure.microsoft.com/en-us/products/machine-learning) platform and launch Azure Machine learning studio.
2. Once the studio is launched go to the compute section and choose a compute instance. The compute instace which I choosed has the following specifications Standard_E8s_v3 
   (8 cores, 64 GB RAM, 128 GB disk).
3. After the compute instance is created launch the jupyter notebook which can be found again in the compute section.
4. Install the packages which I mentioned above and run the "Ddos.pynb" file.
