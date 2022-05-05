# The Future of Computational Microeconomics: Comments for "[Voting-Based Decentralized Consensus Design for Improving the Efficiency and Security of Consortium Blockchain](https://doi.org/10.1109/jiot.2020.3029781)"

> *Disclaimer: Submissions to the Final Project for [COMPSCI/ECON 206 Computational Microeconomics](https://ce.pubpub.org/), 2022 Spring Term (Seven Week - Second) instructed by [Prof. Luyao Zhang](http://scholars.duke.edu/person/luyao.zhang) at Duke Kunshan University.*

## Citation of the Article 

Sun, Gang, Miao Dai, Jian Sun, and Hongfang Yu. 2021. "Voting-Based Decentralized Consensus Design for Improving the Efficiency and Security of Consortium Blockchain." IEEE Internet of Things Journal 8 (8): 6257–72. https://doi.org/10.1109/jiot.2020.3029781.

in BibTex
```
@ARTICLE{9219122,
  author={Sun, Gang and Dai, Miao and Sun, Jian and Yu, Hongfang},
  journal={IEEE Internet of Things Journal}, 
  title={Voting-Based Decentralized Consensus Design for Improving the Efficiency and Security of Consortium Blockchain}, 
  year={2021},
  volume={8},
  number={8},
  pages={6257-6272},
  doi={10.1109/JIOT.2020.3029781}}

```

## 

## Part I: Summary

![Mindmap of Summary](./mindmap.png)


**Fig.1 - Summary Mindmap** created by Whimsical


### 1. Background and Motivation

Consortium blockchain has been gaining increasing attention with the advantages of decentralization, transparency, traceability, and the ability to be tamper-proof theoretically. It is still facing a set of dilemmas in the practical application, such as high energy consumption, time inefficiency, low transaction throughput, poor security, poor user revenue fairness, which hindered the further development of blockchain technology and application [(Sun et al. 2020)](https://doi.org/10.1109/jiot.2020.3029781). Specifically, each participant maintains a copy of the blockchain account book and has equal access to transaction records in a decentralized system. That puts forward higher requirements for managing the consistency of different account books and determining who is responsible for generating new blocks or judging whose blocks are reasonable and legitimate practical decisions. That makes up the core module of alliance blockchain -- consensus algorithm. The consensus algorithm is a fault-tolerant mechanism that is used in computer and blockchain systems to achieve the necessary agreement on a single data value or a single state of the network among distributed processes or multi-agent systems [(Frankenfield 2019a)](https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp). Its efficiency and effectiveness directly affect the performance of the system. However, the current consensus algorithm can not fully match the requirements of technological development. To solve the related problems, this paper proposes a new consensus algorithm, mainly answering how to improve the efficiency and security of the consortium blockchain to improve the performance of the blockchain platform via optimizing the quality of the core modules. 

### 2. Research Questions

How to improve the efficiency and security of consortium blockchain?

### 3. Methods

The paper adopts the Model & Simulation method. It proposes a new algorithm, voting-based decentralized consensus (VDC), to improve the weakness of the existing algorithms [(Sun et al. 2020)](https://doi.org/10.1109/jiot.2020.3029781). First, the model classifies the nodes into different categories, limiting the authority to avoid monopoly and reducing communication complexity. Secondly, based on verifiable random function (VRF), which refers to producing publicly verifiable and unpredictable random values [("Verifiable Random Function" 2021)](https://en.wikipedia.org/wiki/Verifiable_random_function), the algorithm includes the operation of "lottery drawing" to avoid targeted attacks. Thirdly, owners can frequently switch to ensure the algorithm's fairness; Finally, the algorithm takes assets and reputation as rewards and punishments to establish a strict reward and punishment mechanism to regulate user behavior. In this paper, the performance of the VDC algorithm is analyzed theoretically according to the above characteristics. The influence of different parameters on VDC algorithm performance is studied through simulation experiments to ensure performance improvement. Furthermore, the simulation process also compares the VDC algorithm with Practical Byzantine Fault Tolerance (PBFT) and Mixed Byzantine Fault Tolerance (MBFT) algorithms. It proves that the algorithm has apparent advantages in user benefit fairness, time efficiency, and elasticity against target attack and has acceptable extra cost in energy consumption.

### 4. Intellectual Merits

This paper reviews the formation and development of existing major consensus algorithms and points out the corresponding application limitations. Proof of Work (PoW) is an original consensus algorithm that requires effort in solving mathematical puzzles. It is used to operate at the cost of additional CPU consumption, higher time cost, and lower system throughput, which cannot cope with the quality of service requirements of some scenarios [(Frankenfield 2021)](https://www.investopedia.com/terms/p/proof-stake-pos.asp). Besides, Proof of Stake (PoS) is another instrument to achieve consensus requiring participants to stake coins or set them aside to be randomly selected as a validator [(Frankenfield 2019b)](https://www.investopedia.com/terms/p/proof-stake-pos.asp), faces the problem with the decentralization of authority. Another algorithm, the Byzantine Fault Tolerance (BFT) algorithm, carries the computer system's ability to continue operating even some of the nodes fail or act maliciously [(Daly 2021)]( https://www.fool.com/investing/stock-market/market-sectors/financials/cryptocurrency-stocks/byzantine-fault-tolerance/). However, it is also limited by the size of participants, resulting in low system capacity and appointing leaders vulnerable to targeted attacks. At the same time, the fairness of user profit has not reached the expected level of attention. Based on the above research results and problems, this paper formulated the algorithm, voting-based decentralized consensus (VDC) of the consortium blockchain to reach better fairness in terms of user benefits and time efficiency under the condition of acceptable energy consumption without sacrificing security [(Sun et al. 2020)](https://doi.org/10.1109/jiot.2020.3029781). 

In general, the main contributions made by the new consensus algorithm include: 

- In the new consensus model, different nodes will be assigned different identities, enjoying different functions and dealing with different things. Identities can be converted to each other to limit and disperse authority to avoid monopoly; 

- The new strategy determines the privileges and ownership of the packaged blocks, which utilize the dual characteristics of unpredictability and verifiable blockchain, assisting in improving the system's strength against the targeted attacks.

- Based on the existing consensus algorithm that uses reputation and credit as incentive measures, the asset factor is introduced to the algorithm to further increase the cost of malicious behavior and improve the algorithm's security. 

### 5. Practical Impacts

The new consensus algorithm is expected to solve the drawbacks of the existing blockchain algorithms or update the current consensus algorithm to improve the performance of the blockchain platform. However, as a newly born partial theoretical algorithm mechanism, VDC also needs further experiments and improvements to adapt to highly complex application scenarios [(Sun et al. 2020)](https://doi.org/10.1109/jiot.2020.3029781). 

## Part II: Critics 
![Mindmap of Critics](./mindmap2.png)


**Fig.2 - Critics Mindmap** created by Whimsical


### 1. Economics for Computer Science: Incentives in Computer Science

Based on the existing consensus algorithm using reputation and credit as incentive measures, the asset factor is introduced to increase the cost of malicious behavior and further improve the algorithm's security. For example, if a verifier's judgment differs from that of the majority, he is judged to have made the wrong decision, the deposit he previously paid will be awarded to the person who made the proper judgment, and the value of his credit list will be reduced.  

This method combines the dual factors of credit and assets to reward and punish users, which further standardizes users' behavior and strengthens their awareness of rules. In algorithm design, we should also learn from this method and set factors of different dimensions to enhance the influence of user behavior to achieve multi-directional control.  

In addition to reputation and assets, the consideration of rewards and punishments can be further increased, and the relevant mechanisms need to be further improved. Defining "crime cost" can better constrain users is also an important topic.  

### 2. Computer Science for Economics: Practicality in Economics

In this paper, the algorithm's security is described in detail in combination with computer applications. According to common security problems encountered in a specific practice, including Double Spending, Packing, and Targeted Attacks, the author analyzes how the FDC algorithm can solve these security problems better. Thus, the reliability of the algorithm model in practical application is verified. 

The algorithm references the "lottery" step based on VRF so that the algorithm can effectively use the randomness of the computer to determine the slot owner to protect him from targeted attacks. At the same time, it also improves the fairness of users' income in frequent owner switching. 

Excessive randomness in the system may increase system uncertainty and risk, and frequent slot owner changes may lead to unnecessary power consumption. 

## Part III: Inspirations


![Mindmap of Inspirations](./mindmap3.png)


**Fig.1 - Inspirations Mindmap** created by Whimsical


### 1. Interdisciplinary Research

Computational Economics is an integral part of computers and artificial intelligence development. As an essential research tool in economics, game theory is usually used to study how companies adopt appropriate business strategies in market competition to achieve desired goals. The introduction of game theory into computer science is due to the emergence of the Internet and other open networks. Under such a situation, how do we create a second intelligence? A significant problem to solve is how to deal with interactions with other non-human agents [(Dafoe 2021)](https://doi.org/10.1038/d41586-021-01170-0). There are many different strategic interactions between entities in the open web application. Each entity has another rationale and has its interests. According to the actual environment beneficial to itself, each entity decides on a strategy to realize the maximization of attractions; these strategies eventually reach a limited equilibrium state. Like expert systems, writing many rules isn't a good option because that intelligence doesn't scale very well. We hope to give the agent some basic rules of behavior to reflect its personality in the interaction and learn their skills. So how do you set these learning rules? One great tool is game theory. For example, in Game Theory, a multi-agent system can provide a lot of inspiration for solving existing problems, such as designing the benefits and preferences of agents so that they can learn cooperative behaviors. Take the classic case, prisoner's dilemma, for instance, it is best for both parties not to betray, but an intelligent agent that only cares about itself will only cross. 

### 2. Research for Real-world Practices

With the progress of AI technology, more and more problems can be solved by artificial intelligence, and so can game problems. In the future, in-depth research on AI decision-making is expected to be an essential development direction, and game theory is a theoretical framework used to describe and analyze the interaction between multiple agents. According to the different nature of the problem, the game theory can be summarized into the following two solutions for ai decision making: One is entirely based on game theory, that is, the whole problem is modeled as a game process, and then the equilibrium is solved. It should be noted that game solving is often a large-scale optimization problem, requiring a lot of operational research and optimization techniques. Another idea is to use reinforcement learning techniques to solve problems. It is appropriate and necessary to adopt non-model-based reinforcement learning when the problem cannot be well modeled by game theory, the scale is too large, or it is challenging to use optimization methods for non-convex problems.

The development of artificial intelligence is creating new possibilities for game theory. Artificial intelligence provides unique solutions for game theory at the theoretical level. Take Nash equilibrium and equilibrium in cooperative game theory as examples, both of which have some difficulties in computational complexity. It is usually necessary to solve a specific problem with a particular structure in traditional research. At the same time, q-learning and other methods in reinforcement learning have brought new ideas to the calculation of equilibrium. Artificial intelligence has also been applied to go games in some practical applications. Different game scenarios, such as AlphaGo, supported by powerful computing power AlphaStar obtained excellent strategies through the deep reinforcement learning method. They defeated the top human players in the man-machine game confrontation. Moreover, artificial intelligence and reinforcement learning also provide new power for studying game problems in the price war auction and other scenarios.

### 3. Future Professional Growth

Computer science and economics intersect academically, especially in areas where there is a lot of math involved in the two disciplines, such as Algorithmic game theory, computational mechanism design, and Multi-agent systems. The future professional development trajectory can be seen in the applications of the mentioned fields. For instance, user-generated content sites like Zhihu can combine algorithms from computer science with mechanism design from economics when considering content ranking [(Ghosh and Hummel 2014)](https://doi.org/10.1016/j.jet.2014.09.009). 

---
### **Cooporative AI Glossary Table**

| Glossary | Definition |Source|
| ----------- | ----------- |-----------|
| **Consortium blockchains** | **Consortium blockchains** are created and used by groups of corporations when they want to enjoy the advantages in exchanging value and information offered by a distributed ledger but find public, permissionless blockchains inadequate for any reason. |[(“Consortium Blockchain | CoinMarketCap” n.d.)](https://coinmarketcap.com/alexandria/glossary/consortium-blockchain) |
| **Consensus Algorithm** | **Consensus Algorithm** is a fault-tolerant mechanism that is used in computer and blockchain systems to achieve the necessary agreement on a single data value or a single state of the network among distributed processes or multi-agent systems |[(Frankenfield 2019a)](https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp) |
| **Proof of Work (PoW)** | **Proof of Work (PoW)** as an original consensus algorithm that requires effort solving mathematical puzzles is used to operate at the cost of additional CPU consumption, higher time cost, and lower system throughput, which cannot cope with the quality of service requirements of some scenarios |[(Frankenfield 2021)](https://www.investopedia.com/terms/p/proof-stake-pos.asp)|
| **Proof of Stake (PoS)** | **Proof of Stake (PoS)** as another instrument to achieve consensus requiring participants to stake coins or set them aside to be randomly selected as a validator |[(Frankenfield 2019b)](https://www.investopedia.com/terms/p/proof-stake-pos.asp)|
| **Byzantine Fault Tolerance (BFT)** |  **Byzantine Fault Tolerance (BFT)**  algorithm, carrying the computer system's ability to continue operating even some of the nodes fail or act maliciously |[(Daly 2021)]( https://www.fool.com/investing/stock-market/market-sectors/financials/cryptocurrency-stocks/byzantine-fault-tolerance/) |
| **Practical Byzantine Fault Tolerance (PBFT)** |  **Practical Byzantine Fault Tolerance (PBFT)** provides the network with Byzantine state machine approach, meaning implementing a Byzantine Fault Tolerance by copying servers and synchronizing client interactions with server copies. PBFT can ensure the networks fault-tolerance while allowing it to process thousands of operations per second with almost negligible increases in waiting time. |[((“Practical Byzantine Fault Tolerance (PBFT) - BitcoinWiki” n.d.))]( https://en.bitcoinwiki.org/wiki/PBFT) |
| **Mixed Byzantine Fault Tolerance (MBFT)** |  **Mixed Byzantine Fault Tolerance (MBFT)** MBFT uses sharding and layered technology. MBFT functionally partitions the nodes that participate in the consensus process and improves the scalability and efficiency without sacrificing security. MBFT also introduces a random node selection mechanism and a credit mechanism to improve security and fault tolerance. |[((Du, Chen, and Ma 2020))]( https://www.researchgate.net/publication/341314780_MBFT_A_New_Consensus_Algorithm_for_Consortium_Blockchain) |
| **Verifiable Random Function (VRF)** | **Verifiable Random Function (VRF)** refers to produces publicly verifiable and unpredictable random values |[(“Verifiable Random Function” 2021)](https://en.wikipedia.org/wiki/Verifiable_random_function)|

---
### Revision of the final project

- In response to the comments on the jargon explanations, I have given the full name and added the definition for technical words, including "consortium blockchain," "VRF," "PoW," "PoS," and so on. I also created a jargon table and listed the definitions to make it more straightforward for the readers.

- Moreover, I have added citations for the technical word definition and critical sentences from the original paper in terms of more citations. I have further developed the Background and Intellectual Merits sections to explain what other works this paper is based on and what area of research this paper is contributing to.

- Regarding the third question in part III, I have rearranged my original answer to part II and written a new answer as the direction of my professional development, which might fit the requirement better. I have mentioned how my takeaway from this course will benefit me in my professional studies in the future.

> *Original comments form Lewis Tian:
> Natalie’s final project draft is already a complete, well-written version that not only gives a concise summary of the paper but also her original thoughts in the critique. I highly appreciate the clarity, comprehensiveness, and professionalism demonstrated in her final project.
To elaborate, the flow charts offer neat overviews of her points that follow certain logical flows. I especially appreciate her ability to summarize highly technical content into concisely organized points as presented in her summary.
>In addition, her summary and other two parts cover a comprehensive set of points without redundant repetitions, making it engaging for readers.
Moreover, from my perspective, her professionalism is demonstrated in her excellent word choice, use of logical connectors, structure (e.g., the use of numbered lists to clearly express points), and ability to make her points with concrete explanations and examples.
Nicely done!
>While this version is already great work, I would make the following suggestions to improve it to perfection.
First, adding explanations to jargon that are essential for understanding a sentence would be super helpful for making the writing more self-content. For example, in the very first sentence, it might be good to add a footnote to briefly define “consortium blockchain”. The same point can be made for the acronyms in the Methods section. Things like VRF, PBFT, and MBFT should at least be spelled out in their first occurrences.
Second, as Prof. Zhang mentioned in class to all of us, certain parts of the final project need more citations to make a point. For instance, the Background and Intellectual Merits sections can be improved by adding citations to explain what other works this paper is based on and what area of research this paper is contributing to.
>Third, while Natalie’s answers to the first two questions of part III are brilliant and inspiring, for the third question, the current answer, though provides an excellent argument detailing the practical applications of AI and reinforcement learning, might be a bit off the topic of “professional growth”. Natalie could perhaps improve this specific answer by thinking about “what’s your takeaway from this class for future professional growth?”, as instructed. In other words, she should shed more light on how this course contributes in any way to her future professional growth.

---

### References
Bibliography “Consortium Blockchain | CoinMarketCap.” n.d. CoinMarketCap Alexandria. Accessed May 5, 2022. https://coinmarketcap.com/alexandria/glossary/consortium-blockchain.

Dafoe, Allan, Yoram Bachrach, Gillian Hadfield, Eric Horvitz, Kate Larson, and Thore Graepel. 2021. “Cooperative AI: Machines Must Learn to Find Common Ground.” Nature 593 (7857): 33–36. https://doi.org/10.1038/d41586-021-01170-0.

Daly, Lyle. 2021. “What Is Byzantine Fault Tolerance?” The Motley Fool. November 10, 2021. https://www.fool.com/investing/stock-market/market-sectors/financials/cryptocurrency-stocks/byzantine-fault-tolerance/.

Du,Mingxiao, Qijun Chen, and Xiaofeng Ma. 2020. “MBFT: A New Consensus Algorithm for Consortium Blockchain.” IEEE Access 8: 87665–75. https://doi.org/10.1109/access.2020.2993759.

Frankenfield, Jake. 2019a. “Consensus Mechanism (Cryptocurrency).” Investopedia. 2019. https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp.
———. 2019b. “Proof of Stake (PoS).” Investopedia. August 11, 2019. https://www.investopedia.com/terms/p/proof-stake-pos.asp.
———. 2021. “Proof of Work.” Investopedia. March 29, 2021. https://www.investopedia.com/terms/p/proof-work.asp.

Ghosh, Arpita, and Patrick Hummel. 2014. “A Game-Theoretic Analysis of Rank-Order Mechanisms for User-Generated Content.” Journal of Economic Theory 154 (November): 349–74. https://doi.org/10.1016/j.jet.2014.09.009.

“Practical Byzantine Fault Tolerance (PBFT) - BitcoinWiki.” n.d. En.bitcoinwiki.org. Accessed May 5, 2022. https://en.bitcoinwiki.org/wiki/PBFT.

Sun, Gang, Miao Dai, Jian Sun, and Hongfang Yu. 2020. “Voting-Based Decentralized Consensus Design for Improving the Efficiency and Security of Consortium Blockchain.” IEEE Internet of Things Journal 8 (8): 1–1. https://doi.org/10.1109/jiot.2020.3029781.

“Verifiable Random Function.” 2021. Wikipedia. September 27, 2021. https://en.wikipedia.org/wiki/Verifiable_random_function.

### References in BibTex
```
@misc{frankenfield_2019_consensus,
  author = {Frankenfield, Jake},
  title = {Consensus Mechanism (Cryptocurrency)},
  url = {https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp},
  year = {2019},
  organization = {Investopedia}
}

@misc{frankenfield_2021_proof,
  author = {Frankenfield, Jake},
  month = {03},
  title = {Proof of Work},
  url = {https://www.investopedia.com/terms/p/proof-work.asp},
  year = {2021},
  organization = {Investopedia}
}

@misc{frankenfield_2019_proof,
  author = {Frankenfield, Jake},
  month = {08},
  title = {Proof of Stake (PoS)},
  url = {https://www.investopedia.com/terms/p/proof-stake-pos.asp},
  year = {2019},
  organization = {Investopedia}
}

@misc{daly_2021_what,
  author = {Daly, Lyle},
  month = {11},
  title = {What Is Byzantine Fault Tolerance?},
  url = {https://www.fool.com/investing/stock-market/market-sectors/financials/cryptocurrency-stocks/byzantine-fault-tolerance/},
  year = {2021},
  organization = {The Motley Fool}
}

@article{dafoe_2021_cooperative,
  author = {Dafoe, Allan and Bachrach, Yoram and Hadfield, Gillian and Horvitz, Eric and Larson, Kate and Graepel, Thore},
  month = {05},
  pages = {33–36},
  title = {Cooperative AI: machines must learn to find common ground},
  doi = {10.1038/d41586-021-01170-0},
  url = {https://www.nature.com/articles/d41586-021-01170-0},
  volume = {593},
  year = {2021},
  journal = {Nature}
}

@article{sun_2020_votingbased,
  author = {Sun, Gang and Dai, Miao and Sun, Jian and Yu, Hongfang},
  pages = {1-1},
  title = {Voting-based Decentralized Consensus Design for Improving the Efficiency and Security of Consortium Blockchain},
  doi = {10.1109/jiot.2020.3029781},
  urldate = {2020-10-24},
  volume = {8},
  year = {2020},
  journal = {IEEE Internet of Things Journal}
}

@misc{a2021_verifiable,
  month = {09},
  title = {Verifiable random function},
  url = {https://en.wikipedia.org/wiki/Verifiable_random_function},
  urldate = {2022-05-04},
  year = {2021},
  organization = {Wikipedia}
}

@article{ghosh_2014_a,
  author = {Ghosh, Arpita and Hummel, Patrick},
  month = {11},
  pages = {349-374},
  title = {A game-theoretic analysis of rank-order mechanisms for user-generated content},
  doi = {10.1016/j.jet.2014.09.009},
  urldate = {2020-03-29},
  volume = {154},
  year = {2014},
  journal = {Journal of Economic Theory}
}

@misc{consortium,
  title = {Consortium Blockchain | CoinMarketCap},
  url = {https://coinmarketcap.com/alexandria/glossary/consortium-blockchain},
  urldate = {2022-05-05},
  organization = {CoinMarketCap Alexandria}
}

@misc{practical,
  title = {Practical Byzantine Fault Tolerance (pBFT) - BitcoinWiki},
  url = {https://en.bitcoinwiki.org/wiki/PBFT},
  urldate = {2022-05-05},
  organization = {en.bitcoinwiki.org}
}

@article{du_2020_mbft,
  author = {Du, Mingxiao and Chen, Qijun and Ma, Xiaofeng},
  pages = {87665-87675},
  title = {MBFT: A New Consensus Algorithm for Consortium Blockchain},
  doi = {10.1109/access.2020.2993759},
  urldate = {2020-07-04},
  volume = {8},
  year = {2020},
  journal = {IEEE Access}
}
```


