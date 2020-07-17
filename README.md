# Web3 Spatial Research Group | KERNEL Fellowship, Genesis Block


The KERNEL Fellowship is an invite-only fellowship for top tech talent looking to build relationships and products in blockchain and Web3. Hosted by Gitcoin, the program exposes fellows to some of the top minds in the Ethereum community while building skills in critical thinking, strategy, design and development.

The Web3 Spatial Research Group is a multidisciplinary team of KERNEL Fellows investigating opportunities at the intersection of Web3 and spatial data technologies to improve measures of human dignity and planetary stewardship.

We believe that innovations at the convergence of these technologies might enable new, durable tools and mechanisms to re-align human and organizational incentives towards social and environmental objectives. 

- Decentralized spatial finance applications could tie financial incentives to pro-environmental results for firms or reward individuals for preserving ecological health. 
- Enclave computing could disrupt conventional theories of interstate cooperation, and trusted IoT could play a part in creating robust maritime governance systems, including - sanctions enforcement. 
- Smart contracts could enable a global system for the coordination of autonomous vehicles.

Our aim is to understand the intricacies and challenges of this field, and make our learnings available by publishing our research and development efforts. We intend to take both theoretical and applied approaches, researching the technical, social, political and economic factors relating to these technologies, and building functional prototypes to assess the feasibility of identified solutions.

The team has a background in a range of relevant areas, including Web3 strategy, blockchain development, product design, crypto-economic mechanism design, game theory, software engineering and data science. We will look critically at a range of decentralized and privacy-preserving technologies, including consensus networks, smart contracts, secure enclaves and cryptographic protocols.

We are open to feedback, advice, connections, funding - we are open. Please reach out if you would like to get involved, share your perspective, or engage in any way.

---

# Research + Development Tracks
Spatial DeFi
----------

Investigating the use of smart contracts and Web3 technologies in spatial finance, which “uses spatial data technologies to inform financial theory and practice”.

The idea is to use spatial data (i.e. satellite imagery, or measurements collected from connected sensors) to create  pro-environmental incentives using blockchain, smart contracts and other Web3 technologies. Spatial finance is an active field of research, and key to a lot of the emerging sustainable finance work - see Spatial Finance Initiative, Sustainable Finance at Oxford, Green Finance Institute.

Our goal will be to produce research papers and experimental prototypes investigating opportunities in this space. A Decentralized Spatial Finance primer would be appropriate, which would introduce concepts of consensus networks and smart contracts to a green finance audience, along with some of the challenges (oracles being a major one). We will also build some prototypes. Our team will work out the prototypes to build - but two examples illustrate the potential. 

First is a smart contract implementation of a loan for a factory near a river, where the interest rate is calculated based on water quality downstream of the factory. If pollution goes up, so does the interest rate, and vice versa. A second is to use outputs of spatial analytics algorithms estimating, say, carbon emissions or deforestation in an area (based on satellite imagery), and to pay certain accounts based on the change over time. Pay a cement factory to lower CO2 emissions, or a community to keep forests healthy. Dr Caldecott from Oxford in The Economist in May: “We can create smart contracts between a smallholder farmer and a funder where the payment is unlocked if the tree is still there,”

The next level up is to look at how we could  design a net zero carbon market built on smart contracts, as described in this paper.

We are hoping to get some advice and guidance from the Oxford Sustainable Finance Programme. We have also spoken with Christophe Christiaen, Sustainable Finance Lead at the Satellite Applications Catapult. He says they’re really interested in blockchain / smart contracts but haven’t done any work yet on them, due to lack of capacity / knowledge.

The Astral Protocol  
-------------------

A self-sovereign spatial data registry -or- borders on the blockchain. 
 
A system for individuals and organizations like governments and companies to autonomously and transparently make location data about their policy zones available.
The idea is to store geographic boundaries on chain in a way that their administrators control the data (using DIDs). 
 
We’ve built two prototypes with London Blockchain Labs - one for Hyperaware and one at ETHLondon called Geolocker. (The first used Ethereum and Arweave, the second Ethereum and 3Box / IPFS.)
 
It has a lot of interesting applications, especially for autonomous vehicles. The best example we’ve found illustrating why it would be useful is DJI’s Geo Zones. DJI drones have geographic information (polygons) about where they are not allowed to fly - near airports, military bases, etc. This is cool - but it is only possible because DJI is so big - governments couldn’t coordinate with the many firms wanting to enter their markets, and likewise with companies wanting to sell drones (or autonomous cars) in jurisdictions … but with a smart contract bridge, everyone has one place to look to get zone geometries and policy information. Govts update one place - drones always fetch from one place, no matter where they are in the world. Here’s a deck illustrating what we mean.
 
What’s next?
- Writing a light paper / white paper
- Thinking about sovereignty (i.e. who is the ultimate authority in a jurisdiction - or how subordinate levels are handled) and topology (how to identify when zones are adjacent, recognizing overlap / disputes, etc)
- Validating with potential users, considering regulatory / legal issues, etc. 
- Thinking about advanced applications like location-based taxation, location-weighted voting i.e. vote weighting based on where people spend their time, etc.
Commercialization? Is this commercializable? 
- How could this be adopted? It is very much a government play.
 
This is a component of some ideas we have about how to create a governance regime for autonomous weapons based on smart contracts, consensus networks and enclave computing …

Hyperaware
----------
A spatial governance protocol for connected devices. 
 
Governing location-aware connected sensors - autonomous vehicles, IoT devices, phones, etc - based on their location in space. Self-sovereign users, optionally privacy-preserving.
 
This project won the Arweave challenge, and got third in the SAP challenge at the Future of Blockchain 2020 competition. With London Blockchain Labs, we built an alpha implementation of the protocol on Ethereum, Arweave,  IoTeX and Intel SGX using React, Mapbox and NodeJS. The idea is to enforce policies on location-enabled devices based on where they are. This came out of prior work studying maritime security, and learning about how vessels evade international sanctions by spoofing or switching off their location services (like AIS).
 
Easiest use case is congestion zones. When a vehicle drives into a zone, Hyperaware detects that it is within the zone polygon and invokes a smart contract, transferring the congestion charges to the zone owner (for example). Zone owners register DIDs on Ethereum / Arweave, which represent the policy zones under their control - they are self sovereign and (theoretically) can keep zone geometries private. (This is  the Astral Protocol.) Vehicle owners register vehicles on IoTeX (again with DIDs) and stake funds. Vehicles stream points into a secure enclave, where we test to see if they’re inside a zone - if so, we transfer part of that vehicle’s stake into the zone owner’s wallet. Also looking at alerting accounts using proxy re-encryption (i.e. transferring information instead of money.)
 
Lots of use cases with shipping, autonomous cars, UAVs, etc. Again, really interested in investigating how this might pave the way for a way to govern autonomous weapons, preventing them from shooting missiles into peaceful areas, for example. (Obvs significant compliance questions here …)
 
We have had some interest from the Marine Stewardship Council to authenticate that fishing vessels haven’t entered Marine Protected Areas using secure enclaves, and from a large insurance brokerage to do research and possible prototyping on the use of enclaves in insurance. We partnered with IoTeX for the project and have good contacts there. Arweave is also keen to support, if we had a plan to move things forward.
 
What’s next?
- Strategy, commercialization, idea validation - a complete review
- White paper
- Rebuilding the code? Building out smart contract functionality.
- This is where we came up with the Astral Protocol - solves a problem for zone administrators - so  is a part of it.
