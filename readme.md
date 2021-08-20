# A Survey on Natural Language Generation in Task-Oriented Dialogue System: Recent Advances and New Frontiers

![](https://img.shields.io/badge/Status-building-brightgreen) ![](https://img.shields.io/badge/PRs-Welcome-red) 

This repository contains a list of papers, open-sourced codes, datasets and leaderboards in NLG field which is carefully and comprehensively organized. If you found any error, please don't hesitate to open an issue or pull request.




## Contributor

Contributed by [Libo Qin](http://ir.hit.edu.cn/~lbqin/), [Zhouyang Li](https://github.com/RaleLee),  [Jieming Lou](https://github.com/jimmy19991222), [Qiying Yu](https://github.com/yqy2001), [Wanxiang Che](http://ir.hit.edu.cn/~car/).

Thanks for supports from our adviser [Wanxiang Che](http://ir.hit.edu.cn/~car/)!



## Introduction

Natural Language Generation (NLG) in task-oriented dialogue system is a critical component in task-oriented dialogue systems, which has attracted increasing research attention.

NLG aims to convert dialogue acts into natural language responses. The example is shown in the table below: the input contains dialogue act *inform* and slot value pairs (name=Blue Spice, priceRange=low, familyFriendly=yes), and the task of NLG is to transform the input into the corresponding natural language reply: "The Blue Spice is a low cost venue. It is a family friendly location."

| Input  | *inform* （name =  Blue Spice, priceRange =low, familyFriendly = yes） |
| ------ | ------------------------------------------------------------ |
| Output | The Blue Spice is a low cost  venue. It is a family friendly location. |

For the purpose of alleviating pressure in article/dataset collation, we worked on sorting out the relevant data sets, papers, codes and lists of NLG in this project.

At present, the project has been completely open source, including:

1. **NLG domain dataset sorting table:** we sorted out the dataset used in NLG field. You can index in it and get the message of general scale, basic structure, content, characteristics, source and acquisition method of the dataset you want to know.
2. **Articles and infos in different directions in the field of NLG:** we classified and arranged the papers according to the current mainstream frontiers. Each line of the list contains not only the title of the paper, but also the year of publication, the source of publication, the paper link and code link for quick indexing, as well as the dataset used.
3. **Leaderboard list on the mainstream datasets of NLG:** we sorted out the leaderboard on the mainstream datasets. In addition to the paper/model/method name and related scores, each line also has links to year, paper and code if it has.



## Quick path

- [Resources](#resources)

  * [Classic methods](#id_1)
  	* [Templete-based](#id_1_1)
  	* [Plan-based](#id_1_2)
  	* [Class-based](#id_1_3)
  	* [Phrase-based](#id_1_4)
  * [Deeplearning-based Methods](#id_2)
  	* [RNN-based](#id_2_1)
  	* [Seq2Seq-based](#id_2_2)
  	* [Transformer-base](#id_2_3) 

- [Dataset](#dataset)

- [LeaderBoard](#leaderboard)

  

## Resources

<span id='id_1'/>

### 1. Classic methods of task-oriented natural language generation

<span id='id_1_1'/>

### 1.1 Templete-based
&ensp;(1) **NLG vs. Templates**`cs.CL 1995` [[pdf]](https://arxiv.org/pdf/cmp-lg/9504013.pdf)<br>
&ensp;(2) **A versatile system for language generation in conversational system application**`ICSLP 2000` [[pdf]](https://www.isca-speech.org/archive/archive_papers/icslp_2000/i00_3271.pdf)<br>
&ensp;(3) **Natural language generation in the ibm flight information system**`ANLP-NAACL 2000 Workshop` [[pdf]](https://aclanthology.org/W00-0305.pdf)<br>

<span id='id_1_2'/>

### 1.2 Plan-based

&ensp;(1) **SPoT: A trainable sentence planner**`NAACL2001` [[pdf]](https://www.aclweb.org/anthology/N01-1003.pdf)<br>
&ensp;(2) **Training a sentence planner for spoken dialogue using boosting**`Computer Speech & Language 2002` [[pdf]](https://www.cs.ubc.ca/~carenini/TEACHING/CPSC503-05/spot.pdf)<br>
&ensp;(3) **Response planning and generation in the MERCURY flight reservation system**`Computer Speech & Language 2002` [[pdf]](http://groups.csail.mit.edu/sls/publications/2002/mercury.pdf) <br>
&ensp;(4) **Acquiring correct knowledge for natural language generation**`JAIR 2003` [[pdf]](https://www.aaai.org/Papers/JAIR/Vol18/JAIR-1813.pdf)<br>
&ensp;(5) **Trainable sentence planning for complex information presentation in spoken dialog systems**`ACL2004` [[pdf]](https://users.soe.ucsc.edu/~maw/papers/acl04twocolumn.pdf)<br>
&ensp;(6) **Trainable sentence planning system** [[pdf]](https://scienceon.kisti.re.kr/srch/selectPORSrchPatent.do?cn=USP2010067729918) <br>
&ensp;(7) **A probabilistic framework for dialog simulation and optimal strategy learning**`IEEE Transactions on Audio, Speech and Language Processing 2006 `[[pdf]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1597262&tag=1) <br>
&ensp;(8) **An investigation into the validity of some metrics for automatically evaluating natural language generation systems**`ACL 2009` [[pdf]](https://dl.acm.org/doi/pdf/10.1162/coli.2009.35.4.35405) <br>
&ensp;(9) **Individual and domain adaptation in sentence planning for dialogue**`arXiv 2011` [[pdf]](https://arxiv.org/pdf/1111.0048.pdf)<br>
&ensp;(10) **Controlling user perceptions of linguistic style: Trainable generation of personality traits**`ACL 2011` [[pdf]](https://www.aclweb.org/anthology/J11-3002.pdf) <br>
&ensp;(11) **Towards personality-based user adaptation: psychologically informed stylistic language generation** [[pdf]](https://users.soe.ucsc.edu/%7Emaw/papers/umuai2010.pdf) <br>

<span id='id_1_3'/>

### 1.3 Class-based
&ensp;(1)  **Stochastic language generation for spoken dialogue systems** `NAACL 2000` [[pdf]](https://www.aclweb.org/anthology/W00-0306.pdf) <br>
&ensp;(2)  **Bootstrapping lexical choice via multiple-sequence alignment**`EMNLP 2002` [[pdf]](https://www.aclweb.org/anthology/W02-1022.pdf)<br>
&ensp;(3)  **Automatic generation of weather forecast texts using comprehensive probabilistic generation-space models**`Natural Language Engineering 2008` [[pdf]](https://arxiv.org/pdf/1509.01023) <br>

<span id='id_1_4'/>

### 1.4 Phrase-based
&ensp;(1) **Phrase-based statistical language generation using graphical models and active learning**`ACL 2010` [[pdf]](https://www.aclweb.org/anthology/P10-1157.pdf)<br>
&ensp;(2) **Training a natural language generator from unaligned data** `ACL 2015` [[pdf]](https://www.aclweb.org/anthology/P15-1044.pdf) <br>
&ensp;(3) **Imitation learning for language generation from unaligned data**`COLING 2016` [[pdf]](https://www.aclweb.org/anthology/C16-1105.pdf) <br>


<span id='id_2'/>

### 2. Deeplearning-based methods of task-oriented natural language generation

<span id='id_2_1'/>

### 2.1 RNN-based

&ensp;(1) **Stochastic Language Generation in Dialogue using RNN with Convolutional Sentence Reranking**(Restaurant dataset)`Sigdial 2015`[[pdf]](https://arxiv.org/pdf/1508.01755.pdf)<br>
&ensp;(2) **Semantically Conditioned LSTM-based NLG for spoken dialogue systems**(Restaurant/Hotel dataset)`EMNLP 2015`[[pdf]](https://arxiv.org/pdf/1508.01745.pdf)<br>
&ensp;(3) **What to talk about and how? Selective Generation using LSTMs with Coarse-to-Fine Alignment**(WeatherGov/RoboCup dataset)[[pdf]](https://arxiv.org/pdf/1509.00838.pdf)<br>
&ensp;(4) **Toward multi-domain language generation using recurrent neural networks**(Restaurant/Hotel dataset)`NIPS Workshop 2015`[[pdf]](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.704.4246&rep=rep1&type=pdf)<br>
&ensp;(5) **Multi-domain Neural Network Language Generation for Spoken Dialogue Systems**(Restaurant/Hotel/Television/Laptop dataset)`NAACL-HLT 2016` [[pdf]](https://arxiv.org/pdf/1603.01232.pdf)<br>
&ensp;(6) **Neural-based Natural Language Generation in Dialogue using RNN Encoder-Decoder with Semantic Aggregation**(Restaurant/Hotel/Television/Laptop dataset) `SIGDIAL 2017`[[pdf]](https://arxiv.org/pdf/1706.06714.pdf)<br>

<span id='id_2_2'/>

### 2.2 Seq2Seq-based

&ensp;(1) **Sequence-to-Sequence Generation for Spoken Dialogue via Deep Syntax Trees and Strings**(Restaurant dataset) `ACL 2016`[[pdf]](https://arxiv.org/pdf/1606.05491)[[code]](https://github.com/UFAL-DSG/tgen)<br>
&ensp;(2) **A Context-aware Natural Language Generator for Dialogue Systems**(alex context nlg dataset) `SIGDIAL 2016`[[pdf]](https://arxiv.org/pdf/1608.07076.pdf)[[code]](https://github.com/UFAL-DSG/tgen)<br>
&ensp;(3) **A Network-based End-to-End Trainable Task-oriented Dialogue System**(Woz  dataset)`EACL 2017`[[pdf]](https://arxiv.org/pdf/1604.04562.pdf)<br>
&ensp;(4) **Adversarial Domain Adaptation for Variational Neural Language Generation in Dialogue Systems**(Restaurant/Hotel/Television/Laptop dataset) `COLING 2018`[[pdf]](https://arxiv.org/pdf/1808.02586.pdf)<br>
&ensp;(5) **Dual Latent Variable Model for Low-Resource Natural Language Generation in Dialogue Systems** (Restaurant/Hotel/Television/Laptop dataset) `CoNLL 2018`[[pdf]](https://arxiv.org/pdf/1811.04164.pdf)<br>
&ensp;(6) **Variational Cross-domain Natural Language Generation for Spoken Dialogue Systems**(Restaurant/Hotel/Television/Laptop dataset) `Sigdial 2018`[[pdf]](https://arxiv.org/pdf/1812.08879.pdf)<br>
&ensp;(7) **A Deep Ensemble Model with Slot Alignment for Sequence-to-Sequence Natural Language Generation**(Restaurant/Television/Laptop dataset) `NAACL 2018`[[pdf]](https://arxiv.org/pdf/1805.06553.pdf)<br>
&ensp;(8) **A Simple Recipe towards Reducing Hallucination in Neural Surface Realisation**(E2E challenge dataset)`ACL 2018`[[pdf]](https://aclanthology.org/P19-1256.pdf)<br>
&ensp;(9) **Char2char Generation with Reranking for the E2E NLG Challenge**(E2E challenge dataset) `cs.CL 2018`[[pdf]](https://arxiv.org/pdf/1811.05826.pdf)<br>
&ensp;(10) **Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue**(E2E challenge dataset) `EMNLP|IJCNLP 2019`[[pdf]](https://aclanthology.org/D19-1123.pdf)<br>
&ensp;(11) **Constrained Decoding for Neural NLG from Compositional Representations in Task-Oriented Dialogue**(E2E challenge dataset) `ACL 2019`[[pdf]](https://arxiv.org/pdf/1906.07220.pdf)<br>
&ensp;(12) **Retrospective and Prospective Mixture-of-Generators for Task-Oriented Dialogue Response Generation**(Multi-Domain-Woz  dataset)`arXiv 2020`[[pdf]](https://arxiv.org/pdf/1911.08151.pdf)[[code]](https://github.com/Jiahuan-Pei/multiwoz-mdrg)<br>
&ensp;(13) **Template Guided Text Generation for Task-Oriented Dialogue**(E2E challenge /SGD/Multi-Domain-Woz/Multi-Domain-Woz-2.1 dataset)`EMNLP 2020`[[pdf]](https://arxiv.org/pdf/2004.15006.pdf)[[code]](https://github.com/google-research/schema-guided-dialogue)<br>
&ensp;(14) **How to Make Neural Natural Language Generation as Reliable as Templates in Task-Oriented Dialogue**(E2E challenge dataset)`EMNLP 2020|ACL 2020`[[pdf]](http://doras.dcu.ie/25957/1/2020.emnlp-main.230%20%281%29.pdf)[[code]](https://github.com/Henry-E/reliable_neural_nlg)<br>
&ensp;(15) **Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines**(Restaurant/Hotel/Television/Laptop/E2E challenge  dataset)`AAAI 2021`[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf)<br>

<span id='id_2_3'/>

### 2.3 Transformer-based

&ensp;(1) **Semantically Conditioned Dialog Response Generation via Hierarchical Disentangled Self-Attention**(Multi-Domain-Woz  dataset) `ACL 2019`[[pdf]](https://arxiv.org/pdf/1905.12866.pdf)[[code]]( https://github.com/wenhuchen/HDSA-Dialog)<br>
&ensp;(2) **Few-shot Natural Language Generation for Task-Oriented Dialog**(Few-Shot-Woz/Multi-Domain-Woz  dataset)`arXiv 2020`[[pdf]](https://arxiv.org/pdf/2002.12328.pdf)[[code]](https://github.com/pengbaolin/SC-GPT)<br>
&ensp;(3) **Efficient Retrieval Augmented Generation from Unstructured Knowledge for Task-Oriented Dialog**(Multi-Domain-Woz-2.1 dataset)`Workshop of AAAI 2021`[[pdf]](https://arxiv.org/pdf/2102.04643.pdf)[[code]](https://github.com/dthulke/dstc9-track1)<br>
&ensp;(4) **Unstructured Knowledge Access in Task-oriented Dialog Modeling using Language Inference, Knowledge Retrieval and Knowledge-Integrative Response Generation**(Multi-Domain-Woz-2.1 dataset)`arXiv 2021`[[pdf]](https://arxiv.org/pdf/2101.06066.pdf)<br>



## Dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th>Name</th>
    <th>Intro</th>
    <th>Links</th>
    <th>Detail</th>
    <th>Size & Stats</th>
  </tr>
</thead>
<tbody >
<tr>
	<td><code> Restaurant dataset                         </td></code>
		<td> Collected by a spoken dialogue system providing information about certain venues in San Francisco </td>
		<td> Download： https://github.com/shawnwun/RNNLG   Paper： https://arxiv.org/pdf/1508.01745.pdf</td>
		<td> Restaurant Information;Dialogue act types: 8  Slots: 12 Dialogue acts: 248 </td>
		<td> Dialogues: around 1k  Utterances: around 5192   the ratio of training, validation, and testing set: 3:1:1     </td>
</tr>
<tr>
	<td><code> Hotel dataset                          </td></code>
		<td> Collected by a spoken dialogue system providing information about certain venues in San Francisco </td>
		<td> Download： https://github.com/shawnwun/RNNLG   Paper：https://arxiv.org/pdf/1508.01745.pdf</td>
		<td> Hotel Information;Dialogue act types: 8  Slots: 12 Dialogue acts: 164 </td>
		<td> Dialogues: around 1k  Utterances: 5373    the ratio of training, validation, and testing set: 3:1:1            </td>
</tr>
<tr>
	<td><code> Laptop dataset                            </td></code>
		<td> 1. Created by workers recruited by Amazon Mechanical Turk (AMT) by asking them to propose an appropriate natural language realisation corresponding to each system dialogue act actually generated by a dialogue system 2. Enumerated all possible combinations of dialogue act types and slots based on the ontology </td>
		<td> Download： https://github.com/shawnwun/RNNLG    Paper：https://arxiv.org/pdf/1603.01232.pdf</td>
		<td> Laptop Information;Dialogue act types: 14  Slots: 19 Dialogue acts: about 13k</td>
		<td> Dialogues: around 3k  Utterances: 13242  the ratio of training, validation, and testing set: 3:1:1                 </td>
</tr>
<tr>
	<td><code> Television dataset                             </td></code>
		<td> 1. Created by workers recruited by Amazon Mechanical Turk (AMT) by asking them to propose an appropriate natural language realisation corresponding to each system dialogue act actually generated by a dialogue system 2. Enumerated all possible combinations of dialogue act types and slots based on the ontologyo </td>
		<td> Download： https://github.com/shawnwun/RNNLG    Paper： https://arxiv.org/pdf/1603.01232.pdf </td>
		<td> Laptop Information;Dialogue act types: 14  Slots: 16 Dialogue acts: about 7k </td>
		<td> Dialogues: around 2k  Utterances: 7035   the ratio of training, validation, and testing set: 3:1:1                </td>
</tr>
<tr>
	<td><code> E2E challenge dataset                              </td></code>
		<td> 1. Collected using the Crowd-Flower platform. 2. For training end-to-end, data-driven natural language generation systems in the restaurant domain. 3. Homepage: http://www.macs.hw.ac.uk/InteractionLab/E2E/    </td>
		<td> Download:       https://github.com/tuetschek/e2e-metrics  ;           Paper:      https://arxiv.org/pdf/1706.09254.pdf </td>
		<td> Restaurant Information ;However, this dataset has shown more lexical richness and syntactic variation, including discourse phenomena and to generate from this set requires content selection; Dialogue act types: 1  Slots: 8 </td>
		<td> Train：4862 MRs，42061 References     Dev:547 MRs, 4672 References   Teest: 630 MRs, 4693 References              </td>
</tr>
<tr>
	<td><code> Multi-Domain-Woz  dataset                             </td></code>
		<td>  1. a fully-labeled multi-domain collection of human-human written conversations 2.  for Task-Oriented Dialogue Modelling</td>
		<td> Download: https://github.com/budzianowski/multiwoz/blob/master/data/MultiWOZ_2.0.zip   Paper: https://aclanthology.org/D18-1547.pdf </td>
		<td>With dialogues spanning across 7 domains(Attraction, Hospital, Police, Hotel, Restaurant, Taxi, Train) and several topics. Each dialogue is annotated with a sequence of dialogue states and corresponding system dialogue acts </td>
		<td> domains: 7 Dialogues: 8438  Turns: 115424  Slots: 25 Values: 4510                </td>
</tr>
<tr>
	<td><code> Multi-Domain-Woz-2.1  dataset                               </td></code>
		<td> 1. Correct some mistakes in the Multi-Domain-Woz dataset  2. Re-annotate state and utterances based on the original utterances in the dataset  </td>
		<td> Download: https://github.com/budzianowski/multiwoz/blob/master/data/MultiWOZ_2.1.zip         Paper: https://arxiv.org/pdf/1907.01669.pdf </td>
		<td> 1. correction process results in changes to over 32% of state annotations across 40% of the dialogue turns 2. fix 146 dialogue utterances by canonicalizing slot values in the utterances to the values in the dataset ontology </td>
		<td> domains: 7 Dialogues: 10438   Slots: 25 Values: 4510                </td>
</tr></tbody>
</table>
</div>


## LeaderBoard



Restaurant dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Slot-err rate</th>
    <th> BELU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody >
<tr>
	<td><code> IRN(+KNN)                         </td></code>
		<td> 0.11       </td>
		<td> 0.807   </td>
		<td> Slot-consistent NLG for Task-oriented Dialogue Systems with Iterative Rectification Network[[pdf]](https://aclanthology.org/2020.acl-main.10.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> RALSTM                         </td></code>
		<td> 0.16       </td>
		<td> 0.779   </td>
		<td> Paper: Natural Language Generation for Spoken Dialogue System using RNN Encoder-Decoder Networks[[pdf]](https://arxiv.org/pdf/1706.00139.pdf) </td>
		<td> -      </td>
		<td> CoNLL  </td>
		<td></td>
</tr>
<tr>
	<td><code> Softmax                         </td></code>
		<td> 0.20       </td>
		<td> 0.812   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> VQ-VAE                         </td></code>
		<td> 0.18       </td>
		<td> 0.789   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> NLG-LM                         </td></code>
		<td> -       </td>
		<td> 0.795   </td>
		<td> Paper: Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue[[pdf]](https://aclanthology.org/D19-1123.pdf) </td>
		<td> -      </td>
		<td> EMNLP|IJCNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> Gumbel-softmax                         </td></code>
		<td> 0.21       </td>
		<td> 0.776   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> ARoA                         </td></code>
		<td> 0.30       </td>
		<td> 0.776   </td>
		<td> Neural-based Natural Language Generation in Dialogue using RNN Encoder-Decoder with Semantic Aggregation[[pdf]](https://arxiv.org/pdf/1706.06714.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> SCLSTM                         </td></code>
		<td> 0.38       </td>
		<td> 0.753   </td>
		<td> Paper： Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems[[pdf]](https://arxiv.org/pdf/1508.01745.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> EMNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> HLSTM                         </td></code>
		<td> 0.74       </td>
		<td> 0.747   </td>
		<td> Stochastic Language Generation in Dialogue using Recurrent Neural Networks with Convolutional Sentence Reranking[[pdf]](https://arxiv.org/pdf/1508.01755.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
</tbody>
</table>
</div>



Hotel dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Slot-err rate</th>
    <th> BELU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody >
<tr>
	<td><code> NLG-LM                         </td></code>
		<td> -       </td>
		<td> 0.939   </td>
		<td> Paper: Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue[[pdf]](https://aclanthology.org/D19-1123.pdf) </td>
		<td> -      </td>
		<td> EMNLP|IJCNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> Softmax                         </td></code>
		<td> 0.46       </td>
		<td> 0.923   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> VQ-VAE                         </td></code>
		<td> 0.55       </td>
		<td> 0.921   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> IRN(+KNN)                         </td></code>
		<td> 0.32       </td>
		<td> 0.911   </td>
		<td> Slot-consistent NLG for Task-oriented Dialogue Systems with Iterative Rectification Network[[pdf]](https://aclanthology.org/2020.acl-main.10.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> Gumbel-softmax                         </td></code>
		<td> 0.77       </td>
		<td> 0.903   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> RALSTM                         </td></code>
		<td> 0.43       </td>
		<td> 0.898   </td>
		<td> Paper: Natural Language Generation for Spoken Dialogue System using RNN Encoder-Decoder Networks[[pdf]](https://arxiv.org/pdf/1706.00139.pdf) </td>
		<td> -      </td>
		<td> CoNLL  </td>
		<td></td>
</tr>
<tr>
	<td><code> ARoA                         </td></code>
		<td> 1.13       </td>
		<td> 0.892   </td>
		<td> Neural-based Natural Language Generation in Dialogue using RNN Encoder-Decoder with Semantic Aggregation[[pdf]](https://arxiv.org/pdf/1706.06714.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> HLSTM                         </td></code>
		<td> 2.67       </td>
		<td> 0.850   </td>
		<td> Stochastic Language Generation in Dialogue using Recurrent Neural Networks with Convolutional Sentence Reranking[[pdf]](https://arxiv.org/pdf/1508.01755.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> SCLSTM                         </td></code>
		<td> 3.07      </td>
		<td> 0.848   </td>
		<td> Paper： Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems[[pdf]](https://arxiv.org/pdf/1508.01745.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> EMNLP  </td>
		<td></td>
</tr></tbody>
</table>
</div>



Laptop dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Slot-err rate</th>
    <th> BELU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody><tr>
	<td><code> Softmax                         </td></code>
		<td> 0.31       </td>
		<td> 0.591   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> NLG-LM                         </td></code>
		<td> -       </td>
		<td> 0.586   </td>
		<td> Paper: Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue[[pdf]](https://aclanthology.org/D19-1123.pdf) </td>
		<td> -      </td>
		<td> EMNLP|IJCNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> Gumbel-softmax                         </td></code>
		<td> 0.63       </td>
		<td> 0.561   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> VQ-VAE                         </td></code>
		<td> 0.65       </td>
		<td> 0.554   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> IRN(+KNN)                         </td></code>
		<td> 0.29       </td>
		<td> 0.537   </td>
		<td> Slot-consistent NLG for Task-oriented Dialogue Systems with Iterative Rectification Network[[pdf]](https://aclanthology.org/2020.acl-main.10.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> RALSTM                         </td></code>
		<td> 0.42       </td>
		<td> 0.525   </td>
		<td> Paper: Natural Language Generation for Spoken Dialogue System using RNN Encoder-Decoder Networks[[pdf]](https://arxiv.org/pdf/1706.00139.pdf) </td>
		<td> -      </td>
		<td> CoNLL  </td>
		<td></td>
</tr>
 <tr>
 <td><code> Slug2Slug                         </td></code>
		<td> 1.55   </td>
  <td>0.524</td>
		<td> Paper: Slug2Slug: A Deep Ensemble Model with Slot Alignment for Sequence-to-Sequence Natural Language Generation[[pdf]](http://www.macs.hw.ac.uk/InteractionLab/E2E/final_papers/E2E-Slug2Slug.pdf)
</td>
		<td> -      </td>
		<td> -  </td>
<td></td>
</tr>
 <tr>
	<td><code> ARoA  </td></code>
		<td> 0.50       </td>
		<td> 0.522   </td>
		<td> Neural-based Natural Language Generation in Dialogue using RNN Encoder-Decoder with Semantic Aggregation[[pdf]](https://arxiv.org/pdf/1706.06714.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> HLSTM                         </td></code>
		<td> 1.10       </td>
		<td> 0.513   </td>
		<td> Stochastic Language Generation in Dialogue using Recurrent Neural Networks with Convolutional Sentence Reranking[[pdf]](https://arxiv.org/pdf/1508.01755.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> SCLSTM                         </td></code>
		<td> 0.79       </td>
		<td> 0.512   </td>
		<td> Paper： Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems[[pdf]](https://arxiv.org/pdf/1508.01745.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> EMNLP  </td>
		<td></td>
</tr>
</tbody>
</table>
</div>



Television dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Slot-err rate</th>
    <th> BELU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody >
<tr>
	<td><code> NLG-LM                         </td></code>
		<td> -       </td>
		<td> 0.617   </td>
		<td> Paper: Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue[[pdf]](https://aclanthology.org/D19-1123.pdf) </td>
		<td> -      </td>
		<td> EMNLP|IJCNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> Softmax                         </td></code>
		<td> 0.51       </td>
		<td> 0.610   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> VQ-VAE                         </td></code>
		<td> 0.70       </td>
		<td> 0.598   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> Gumbel-softmax                         </td></code>
		<td> 0.79       </td>
		<td> 0.581   </td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> IRN(+KNN)                         </td></code>
		<td> 0.35       </td>
		<td> 0.559   </td>
		<td> Slot-consistent NLG for Task-oriented Dialogue Systems with Iterative Rectification Network[[pdf]](https://aclanthology.org/2020.acl-main.10.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> RALSTM                         </td></code>
		<td> 0.63      </td>
		<td> 0.541   </td>
		<td> Paper: Natural Language Generation for Spoken Dialogue System using RNN Encoder-Decoder Networks[[pdf]](https://arxiv.org/pdf/1706.00139.pdf) </td>
		<td> -      </td>
		<td> CoNLL  </td>
		<td></td>
</tr>
 <tr>
	<td><code> ARoA                         </td></code>
		<td> 0.60       </td>
		<td> 0.539   </td>
		<td> Neural-based Natural Language Generation in Dialogue using RNN Encoder-Decoder with Semantic Aggregation[[pdf]](https://arxiv.org/pdf/1706.06714.pdf) </td>
		<td> -      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
	<td><code> SCLSTM                         </td></code>
		<td> 2.31       </td>
		<td> 0.527   </td>
		<td> Paper： Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems[[pdf]](https://arxiv.org/pdf/1508.01745.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> EMNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> HLSTM                         </td></code>
		<td> 2.50       </td>
		<td> 0.525   </td>
		<td> Stochastic Language Generation in Dialogue using Recurrent Neural Networks with Convolutional Sentence Reranking[[pdf]](https://arxiv.org/pdf/1508.01755.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> Sigdial  </td>
		<td></td>
</tr>
<tr>
 <td><code> Slug2Slug                         </td></code>
		<td> 1.67   </td>
    <td>0.523</td>
		<td> Paper: Slug2Slug: A Deep Ensemble Model with Slot Alignment for Sequence-to-Sequence Natural Language Generation[[pdf]](http://www.macs.hw.ac.uk/InteractionLab/E2E/final_papers/E2E-Slug2Slug.pdf)
</td>
		<td> -      </td>
		<td> -  </td>
</tr>
</tbody>
</table>
</div>



E2E Challenge dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> BELU </th>
    <th> NIST </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody >
 <tr>
	<td><code> OpenNMT                        </td></code>
		<td> 0.681   </td>
    <td> 8.748 </td>
		<td> Paper： How to Make Neural Natural Language Generation as Reliable as Templates in Task-Oriented Dialogue[[pdf]](http://doras.dcu.ie/25957/1/2020.emnlp-main.230%20(1).pdf) </td>
		<td>  https://github.com/Henry-E/reliable_neural_nlg      </td>
		<td>  EMNLP|ACL  </td>
		<td></td>
</tr>
<tr>
	<td><code> TUDA(Model-D)                        </td></code>
		<td> 0.713   </td>
    <td> 8.502 </td>
		<td> Paper： E2E NLG Challenge: Neural Models vs. Templates[[pdf]](https://aclanthology.org/W18-6557.pdf) </td>
		<td>  https://github.com/UKPLab/e2e-nlg-challenge-2017      </td>
		<td> ACL  </td>
		<td></td>
</tr>
<tr>
	<td><code> Softmax                        </td></code>
		<td> 0.697   </td>
<td>-</td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> Slug2Slug                         </td></code>
		<td> 0.662   </td>
  <td>8.613</td>
		<td> Paper: Slug2Slug: A Deep Ensemble Model with Slot Alignment for Sequence-to-Sequence Natural Language Generation[[pdf]](http://www.macs.hw.ac.uk/InteractionLab/E2E/final_papers/E2E-Slug2Slug.pdf)
</td>
		<td> -      </td>
		<td> -  </td>
		<td></td>
</tr>
<tr>
	<td><code> NLG-LM                         </td></code>
		<td> 0.684   </td>
<td>-</td>
		<td> Paper: Multi-task Learning for Natural Language Generation in Task-Oriented Dialogue[[pdf]](https://aclanthology.org/D19-1123.pdf) </td>
		<td> -      </td>
		<td> EMNLP|IJCNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> VQ-VAE                         </td></code>
		<td> 0.681   </td>
<td>-</td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> TGen                         </td></code>
		<td> 0.659       </td>
<td>8.609</td>
		<td> Paper: Sequence-to-Sequence Generation for Spoken Dialogue via Deep Syntax Trees and Strings[[pdf]](https://arxiv.org/pdf/1606.05491.pdf) </td>
		<td> https://github.com/UFAL-DSG/tgen      </td>
		<td> ACL   </td>
		<td></td>
</tr>
<tr>
	<td><code> OpenNMT+Surface Forms                        </td></code>
		<td> 0.628   </td>
    <td> 8.311 </td>
		<td> Paper： How to Make Neural Natural Language Generation as Reliable as Templates in Task-Oriented Dialogue[[pdf]](http://doras.dcu.ie/25957/1/2020.emnlp-main.230%20(1).pdf) </td>
		<td>  https://github.com/Henry-E/reliable_neural_nlg      </td>
		<td>  EMNLP|ACL  </td>
		<td></td>
</tr>
<tr>
	<td><code> Gumbel-softmax                         </td></code>
		<td> 0.667   </td>
<td>-</td>
		<td> Paper: Interpretable NLG for Task-oriented Dialogue Systems with Heterogeneous Rendering Machines[[pdf]](https://www.aaai.org/AAAI21Papers/AAAI-3767.LiY.pdf) </td>
		<td> -      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> TUDA(Model-T)                        </td></code>
		<td> 0.605   </td>
    <td> 7.526 </td>
		<td> Paper： E2E NLG Challenge: Neural Models vs. Templates[[pdf]](https://aclanthology.org/W18-6557.pdf) </td>
		<td>  https://github.com/UKPLab/e2e-nlg-challenge-2017      </td>
		<td> ACL  </td>
		<td></td>
</tr>
</tbody>
</table>
</div>



Multi-Domain-Woz dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Entity F1</th>
    <th> BLEU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody >
  <tr>
	<td><code> SC-GPT                         </td></code>
		<td> 88.37   </td>
    <td> 30.76 </td>
		<td> Paper: Few-shot Natural Language Generation for Task-Oriented Dialog[[pdf]](https://arxiv.org/pdf/2002.12328.pdf) </td>
		<td>  https://github.com/pengbaolin/ SC-GPT      </td>
		<td> arXiv  </td>
		<td></td>
</tr>
 <tr>
	<td><code> GPT-2                         </td></code>
		<td> 87.70   </td>
    <td> 30.71 </td>
		<td> Paper: Few-shot Natural Language Generation for Task-Oriented Dialog[[pdf]](https://arxiv.org/pdf/2002.12328.pdf) </td>
		<td>  https://github.com/pengbaolin/ SC-GPT      </td>
		<td> arXiv  </td>
		<td></td>
</tr> 
 <tr>
	<td><code> HDSA                        </td></code>
		<td> 87.30   </td>
    <td> 26.48 </td>
		<td> Paper： Semantically Conditioned Dialog Response Generation via Hierarchical Disentangled Self-Attention[[pdf]](https://arxiv.org/pdf/1905.12866.pdf) </td>
		<td>  https://github. com/wenhuchen/HDSA- Dialog      </td>
		<td> ACL  </td>
		<td></td>
</tr>
  <tr>
	<td><code> SCLSTM                        </td></code>
		<td> 80.42   </td>
    <td> 21.6 </td>
		<td> Paper： Semantically Conditioned LSTM-based Natural Language Generation for Spoken Dialogue Systems[[pdf]](https://arxiv.org/pdf/1508.01745.pdf) </td>
		<td> https://github.com/shawnwun/RNNLG      </td>
		<td> EMNLP  </td>
		<td></td>
</tr>
<tr>
	<td><code> MoGNet                        </td></code>
		<td> 78.85   </td>
    <td> 20.13 </td>
		<td> Paper: Retrospective and Prospective Mixture-of-Generators for Task-oriented Dialogue Response Generation[[pdf]](https://arxiv.org/pdf/1911.08151.pdf) </td>
		<td>  https://github.com/Jiahuan-Pei/multiwoz-mdrg      </td>
		<td> arXiv  </td>
		<td></td>
</tr>
<tr>
	<td><code> LaRLAttnGRU                         </td></code>
		<td> 80.95   </td>
    <td> 12.80 </td>
		<td> Paper: Global-locally self-attentive encoder for dialogue state tracking[[pdf]](https://aclanthology.org/P18-1135.pdf) </td>
		<td>  -      </td>
		<td> ACL   </td>
		<td></td>
</tr>
<tr>
	<td><code> Structured Fusion                         </td></code>
		<td> 77.04  </td>
    <td> 16.34 </td>
		<td> Paper: Structured fusion networks for dialog[[pdf]](https://arxiv.org/pdf/1907.10016.pdf) </td>
		<td>  -      </td>
		<td> Sigdial   </td>
		<td></td>
</tr>
</tbody>
</table>
</div>



Multi-Domain-Woz-2.1 dataset

<div style="overflow-x: auto; overflow-y: auto; height: auto; width:100%;">
<table style="width:100%" border="2">
<thead>
  <tr>
    <th> Model</th>
    <th> Entity F1</th>
    <th> BLEU </th>
    <th>Paper / Source</th>
    <th>Code link</th>
    <th>Conference</th>
  </tr>
</thead>
<tbody > 
   <tr>
	<td><code> HDNO                         </td></code>
		<td> 87.63   </td>
    <td> 18.97 </td>
		<td> Paper: MODELLING HIERARCHICAL STRUCTURE BETWEEN DIALOGUE POLICY AND NATURAL LANGUAGE GEN- ERATOR WITH OPTION FRAMEWORK FOR TASK- ORIENTED DIALOGUE SYSTEM[[pdf]](https://arxiv.org/pdf/2006.06814.pdf) </td>
		<td>   https://github.com/mikezhang95/HDNO      </td>
		<td> ICLR  </td>
		<td></td>
</tr>
  <tr>
	<td><code> MarCo                        </td></code>
		<td> 84.51   </td>
    <td> 19.54 </td>
		<td> Paper: Multi-Domain Dialogue Acts and Response Co-Generation[[pdf]](https://arxiv.org/pdf/2004.12363.pdf) </td>
		<td> https://github.com/InitialBug/ MarCo-Dialog      </td>
		<td> ACL  </td>
		<td></td>
</tr>
<tr>
	<td><code> LAVA                         </td></code>
		<td> 89.52   </td>
    <td> 14.02 </td>
		<td> Paper: LAVA: Latent Action Spaces via Variational Auto-encoding for Dialogue Policy Optimization[[pdf]](https://www.aclweb.org/anthology/2020.coling-main.41.pdf) </td>
		<td> https://github.com/budzianowski/multiwoz     </td>
		<td> COLING  </td>
		<td></td>
</tr>
  <tr>
	<td><code> UBAR                         </td></code>
		<td> 86.45   </td>
    <td> 16.70 </td>
		<td> Paper: UBAR: Towards Fully End-to-End Task-Oriented Dialog System with GPT-2[[pdf]](https://arxiv.org/pdf/2012.03539.pdf) </td>
		<td> https://github.com/ TonyNemo/UBAR- MultiWOZ      </td>
		<td> AAAI  </td>
		<td></td>
</tr>
<tr>
	<td><code> DoTs                         </td></code>
		<td>  79.93  </td>
    <td> 15.9 </td>
		<td> Paper: Domain State Tracking for a Simplified Dialogue System[[pdf]](https://arxiv.org/pdf/2103.06648.pdf) </td>
		<td> -     </td>
		<td> arXiv  </td>
		<td></td>
</tr>
<tr>
	<td><code> SimpleTOD                         </td></code>
		<td> 78.87   </td>
    <td> 16.22 </td>
		<td> Paper: A Simple Language Model for Task-Oriented Dialogue[[pdf]](https://arxiv.org/pdf/2005.00796.pdf) </td>
		<td>  https://github.com/ salesforce/simpletod      </td>
		<td> arXiv  </td>
		<td></td>
</tr>
 <tr>
	<td><code> LABES-S2S                         </td></code>
		<td>  72.14  </td>
    <td> 18.3 </td>
		<td> Paper: A Probabilistic End-To-End Task-Oriented Dialog Model with Latent Belief States towards Semi-Supervised Learning[[pdf]](https://arxiv.org/pdf/2009.08115.pdf) </td>
		<td> https://github.com/thu-spmi/LABES     </td>
		<td> EMNLP  </td>
		<td></td>
</tr>
</tbody>
</table>
</div>

