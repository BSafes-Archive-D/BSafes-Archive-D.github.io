---
layout: default
title: DDoS – Technical Developments
parent: § DDoS - From Activist Event to Perpetual Crisis 
grand_parent: D 
nav_order: 20 
---
<style>
.dont-break-out {
  /* These are technically the same, but use both */
  overflow-wrap: break-word;
  word-wrap: break-word;

     -ms-word-break: break-all;
  /* This is the dangerous one in WebKit, as it breaks things wherever */
  word-break: break-all;
  /* Instead use this non-standard one: */
  word-break: break-word;
}

.youtube-container {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 56.25%;
}
.youtube-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

</style>

<div class="dont-break-out" markdown="1">

1. TOC
{:toc}

## DDoS – Technical Developments
A DDoS attack seeks to exhaust the capacity of a web server by overwhelming it with requests, thus rendering content inaccessible. Under normal working conditions, a request to a server, initiated by a user, prompts that server to send the requested data. During a successful DDoS attack, a server is unable to distinguish between legitimate requests by regular users and requests that are sent with the purpose of bringing the server down. In trying to fulfil all requests, the server and/or the network eventually meet capacity limits, which means that legitimate requests receive error responses.

***
<sup>6</sup> Molly Sauter, *The Coming Swarm. DDoS Actions, Hacktivism, and Civil Disobedience on the Internet* (New York; London: Bloomsbury Academic, 2014). 
{: .fs-2}
<sup>7</sup> Tim Jordan and Paul Taylor, *Hacktivism and Cyberwars: Rebels with a Cause?* (London; New York: Routledge, 2004), 75-82.
{: .fs-2}
***

Usually, DDoS attacks do not affect the data that is stored on a server, but rather make it temporarily inaccessible. Yet, depending on the scale of the attack, it can take a considerable amount of time and resources to restore the functionality of the system.

Denial of Service has a long legacy as a technique for disturbing online communication and a wide range of different strategies have been developed and implemented. <sup>8</sup> Many of these approaches are well known in the field of computer science and there is an equally active development of counter-strategies for defending servers and networks against them. <sup>9</sup> A key factor in these strategies is the ability to identify patterns in DDoS attack traffic, since such patterns can be used as the basis for developing filtering and blocking rules, as well as more flexible traffic management mechanisms based on Machine Learning. <sup>10</sup> At the same time, there is a constant search for vulnerabilities in online systems that can be exploited for expanding DDoS capabilities. The proliferation of connected devices commonly referred to as the Internet of Things is especially prone to such exploitation, since these devices often lack adequate security features. <sup>11</sup>

The simplest versions of DDoS that rely on sending large numbers of identical requests, so-called volumetric attacks, often produce easily identifiable traffic patterns, which is why most websites today are effectively defended against them. More advanced versions of DDoS rely on application layer attacks. These are based on a strategy where requests are sent in ways that mimic the behaviour of regular users, making it difficult to identify and filter out attack traffic. Two popular kinds of application layer attacks are HTTP flood and reflection attacks. An HTTP flood can be initiated by different kinds of software, from simple scripts to more elaborate and established techniques, where requests for large amounts of data are sent at longer intervals. Some of these techniques are comparatively easy to defend against, since they involve identifiable combinations of IP addresses and user agents that can be blocked. Also, many systems serve cached versions of frequently requested files, which reduces the load on servers and, thus, protects them against simple HTTP floods –

***
<sup>8</sup> Laura DeNardis, “A History of Internet Security”, in *The History of Information Security: A Comprehensive Handbook,* ed. Karl de Leeuw and Jan Bergstra (Amsterdam, London: Elsevier, 2007), 681-704. 
{: .fs-2}
<sup>9</sup> Sajal Bhatia, Sunny Behal, and Irfan Ahmed, “Distributed Denial of Service Attacks and Defense Mechanisms: Current Landscape and Future Directions”, in *Versatile Cybersecurity,* ed. Mauro Conti, Gaurav Somani, and Radha Poovendran (Cham: Springer Nature Switzerland, 2018), 55-97. 
{: .fs-2}
<sup>10</sup> Kian Son Hoon et al., “Critical Review of Machine Learning Approaches to Apply Big Data Analytics in DDoS Forensics”, in *2018 International Conference on Computer Communication and Informatics* (ICCCI), 2018, 1-5. https://doi.org/10.1109/ICCCI.2018.8441286. 
{: .fs-2}
<sup>11</sup> Constantinos Kolias et al., “DDoS in the IoT: Mirai and Other Botnets”, *Computer* 50, no. 7 (2017): 80- 84.
{: .fs-2}
***

which again has triggered the development of counterstrategies on the part of attackers.

Reflection attacks rely on exploiting specific vulnerabilities of systems in order to prompt them to send requests to a target server. Even more advantageous for an attacker are systems that not only reflect, but also amplify traffic, i.e. that send (sometimes considerably) larger amounts of traffic to the target than the attacker sent to the system, thus amplifying bandwidth resources.<sup>12</sup> Beyond the exploitation of such functionalities and vulnerabilities, the spread of malware allows attackers to take complete control over a system, and then instruct them to send requests to a target server or a reflection server. Compromised devices can be gathered into botnets, which receive their instructions from command and control servers. The challenge for the bot herder is then to distribute malware as efficiently as possible, to establish reliant and secure communication to the command and control server, to secure the botnet against being taken over by others and to make it difficult to track down the command and control server that issues instructions. <sup>13</sup>

The example of the DDoS attack against Black Lives Matter illustrates how these developments play out in practice. As a detailed technical investigation shows, <sup>14</sup> botnet commands in this case could be traced back to servers that were rented temporarily from Digital Ocean, a company offering Virtual Private Services and hosted by DMZHOST, a hosting company that keeps the identity of its clients secret. Yet, even if it were possible to identify the clients of these companies, it is not unlikely that they would turn out to be a commercial entity offering DDoS as a service. These services are marketed openly on the web, thinly disguised as “booters” or “stressers” that website owners can use to test the resilience of their systems. <sup>15</sup>

***
<sup>12</sup> Kulvinder Singh and Ajit Singh, “Memcached DDoS Exploits: Operations, Vulnerabilities, Preventions and Mitigations”, in *2018 IEEE 3rd International Conference on Computing, Communication and Security* (ICCCS), 2018, 171-79, https://ieeexplore.ieee.org/document/ 8586810. 
{: .fs-2}
<sup>13</sup> Pascal Geenens, “IoT Botnets. The Journey So Far and the Road Ahead”, in *Botnets: Architectures, Countermeasures, and Challenges,* ed. Georgios Kambourakis et al. (New York: CRC Press, 2020), 33- 100. 
{: .fs-2}
<sup>14</sup> Seamus Tuohy, “Botnet Attack Analysis of Deflect Protected Website Blacklivesmatter.com”, *eQualitie*, December 14, 2016, https://equalit.ie/en/deflect-labs-report-3-3d/. 
{: .fs-2}
<sup>15</sup> Santanna, José Jair, “DDoS-as-a-Service: Investigating Booter Websites” (PhD diss., University of Twente, 2017), https://research.utwente.nl/en/publications/ddos-as-a-service-investigating-booterwebsites.
{: .fs-2}
***

From this – very rough – sketch of developments in the DDoS landscape, three aspects can be singled out as especially pertinent when it comes to DDoS as a political tactic:

### 1. Complexity of motives
The use of reflection tactics, botnets, command and control servers, virtual private services, etc., increases the distance between the attacker and the target, rendering the attribution of attacks ever more difficult, if not impossible. Therefore, performing a DDoS attack involves very little risk of being exposed. However, the different layers of the attack infrastructure are also characterised by a functional differentiation which can be tied to different motives of the involved actors. Some parts, such as commercial booter services or virtual private services, can be primarily driven by financial gain, whereas other parts, such as malware development, can be primarily fuelled by reputation in hacker circles; others still can be based on political motives, both grass-root activist or state-sponsored. <sup>16</sup> The current DDoS landscape is thus characterised by a growing complexity of interlinked motives on different levels of the attack infrastructure.

### 2. Automation and consolidation
The use of botnets represents one aspects of a tendency to automate and consolidate DDoS attack capabilities. Both the identification of vulnerable devices and their recruitment into botnets are processes that are increasingly automated, minimising the manual effort involved in being a bot herder. Increasing automation implies that the administration of these services is becoming less laborious and that there is increased competition between different providers, driving prices down. The resulting availability of pre-packaged attack capabilities as a service means that it requires neither technical expertise nor established contacts nor substantial funds to launch attacks against political opponents. In the words of the technical report on the attacks against Black Lives Matter: “Silencing online voices is becoming ever easier and cheaper on the Internet.” <sup>17</sup>

***
<sup>16</sup> Some authors seek to identify causal historical trajectories from hacktivism to other forms of DDoS, e.g., Tracey Caldwell, “Hacktivism Goes Hardcore”, *Network Security* 2015, no. 5 (1 May 2015): 12-17. The argument here does not follow this line of reasoning, but rather focuses on the intermingling of different motives on different functional layers.
{: .fs-2}
<sup>17</sup> Tuohy, “Botnet Attack Analysis of Deflect Protected Website Blacklivesmatter.com”.
{: .fs-2}
***

### 3. Reliance on professional protection
With the web becoming an increasingly hostile environment, there is a constant risk that attempts will be made at blocking access to the online presence of activist organisations whenever content or actions are perceived as controversial by others. <sup>18</sup> Without professional protection, even simpler attacks have the potential of blocking access to content. This means that activist organisations have to take the possibility of attacks into account and prepare accordingly by soliciting protection from professional providers of IT security. However, relying on these services also means being at the mercy of a provider’s internal policies and business objectives.<sup>19</sup>

Taken together, these three developments suggest an ongoing qualitative shift of DDoS from exceptional disruptions that can work in favour of activists’ political purposes to a situation where DDoS becomes part of the infrastructural conditions of online activism. This shift raises crucial questions about power relations in the digital realm: Under what circumstances can DDoS be perceived as a tactic for activists to unbalance prevailing asymmetries of power and under which circumstances does it instead serve to stabilise such asymmetries or contribute to the establishment of new ones?

***

#### Table of Contents
{: .no_toc}

<ul><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-1/">
Introduction</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-2/">
DDoS – Technical Developments</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-3/">
Phases of Hacktivism</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-4/">
Phases of DDoS: Technological developments</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-5/">
Effectivity and Legitimacy of DDoS</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-6/">
Breakdown and visibility</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-7/">
DDoS as breakdown</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-8/">
DDoS becomes ordinary</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-9/">
The politics of infrastructuring</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-10/">
Conclusions</a></li><li> <a href="/docs/D/DDoS-From-Activist-Event-to-Perpetual-Crisis-11/">
Bibliography</a></li></ul>
***

</div>
