# Domain Name Systems and IP Addresses

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fnetworkencyclopedia.com%2Fwp-content%2Fuploads%2F2019%2F09%2Fdns-server.jpg&f=1&nofb=1" alt="DNS IP Cluster" height="200">

DNS stands for Domain Name Systems which is most closely related to the string of numbers known as IP addresses (192.168.1.1).

DNS takes what you put into a search bar (https://www.facebook.com/) and turns this into a this string of numbers. Translating what we as humans understand in our native language to integers.

Domain Name | IP Address
-------------------------
youtube.com | 20.51.154.170
news.com | 134.25.25.220
markinfo.dev | 125.239.1.2.2

The DNS will search through what you have typed in and convert this to a computer readable IP Address. Once this is done, it allows our computer to access information from this website.

---

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.dribbble.com%2Fusers%2F537941%2Fscreenshots%2F3986187%2Fgif-unit-01.gif&f=1&nofb=1" alt="man search computer" height="200">

> Example

For instance, you are trying to access https://www.google.com/ and your computer has NOT accessed this site before*. A query will be sent to the next level of a resolver server. This server is your ISP and will take what you have sent to its cache memory to locate the IP Address. If this is not found here, we move on to the next level being the root server. 

*Root Server*

The top root of the DNS hierarchy  

* 13 sets of these root servers are placed around the world and are operated by 12 organizations  
* Each set has their own unique IP Address  

The *root* server does not know where the IP Address https://www.google.com/ is but can assist the resolver in locating the IP Address.   

The *resolver* will then be directed to a Top Level Domain (TLD) server. This server stores address information for top level domains such as (.com .org .edu etc.). The TLD will not know this here and will finally move to our last step being the Authoritative Name Server.  

The ANS is responsible for knowing everything about the server that we are trying to access including the main IP address.   
This IP Address will be sent back to the resolver, then communicated with the initial (your) computer. Lastly, this IP is stored in the resolver for further use.   

* Cache (Stored) memory would allow the computer to already convert this DNS from memory 

