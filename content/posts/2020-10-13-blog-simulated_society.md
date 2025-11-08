+++
title = "Simulated Societies"
date = "2020-10-13"
+++

The exponential growth of computing power has carried with it new possibilities
to speed up processes through automation or obtain deeper understandings of
problems unfathomable for the human mind. With it grew the datafication of
spaces, first motivated by governance and now increasingly by capitalism.
Accordingly, a plethora of mathematical procedures have been codified into
algorithms to make use of the data to, for instance visualise trends, find
correlations, and augment reality. In the pursuit of squeezing ever more insight
out of data, different algorithms can be composed in various ways to achieve
certain goals.

One broad class of algorithms, that have gained popularity in the last decade,
are collectively referred to as machine learning (ML) procedures. ML has
undeniably reshaped how social, economic, and political power is created,
exerted, and extended like no other algorithm. ML aims to develop algorithms
which exhibit true or a facsimile of intelligence, which has already shown
beneficial application in, for example transportation through self-driving cars
and healthcare by supporting diagnosis of illnesses.

An algorithm that has hitherto escaped public discourse, which has nonetheless
spread its roots firmly into our social structure, is known as agent-based
modelling (ABM). Its aim is to study emerging phenomena from seemingly chaotic
processes through agents that are equipped with their own attributes and rules.
Since its first successful application within the social sciences in 1971
[[1]](#1), it is seen as a useful tool for applying a complex
systems lens to guide policies in e.g. transportation to reduce traffic and public
health by understanding the social and environmental determinants of well being
[[2]](#2),[[3]](#3),[[4]](#4). Now, propelled by the COVID-19
pandemic, ABM has been brought into the spotlight through its insights of the
viral spread in buildings, cities (e.g. [[5]](#5), [[6]](#6)),
and countries (e.g. [[7]](#7) which has caused UKs policy shift
away from herd immunity). Now on stage, it will likely accelerate the already
existing trend of increased utilisation of ABM as apparent from the statistics
of the Journal of Artificial Societies and Social Simulation ([JASSS](http://jasss.soc.surrey.ac.uk/stats/statistics.html))
and recognition as [UK govt](https://www.gov.uk/government/publications/computational-modelling-blackett-review) and the [IEEE](https://spectrum.ieee.org/artificial-intelligence/medical-ai/why-modeling-the-spread-of-covid19-is-so-damn-hard).

By placing ABM in juxtaposition to ML, we can see how each affects the society
from opposing ends: while ML can optimise the behaviour of a single car, ABM can
optimise the flow of cars. In other words, ML influences society by affecting its
members (bottom-up), ABM influences members by affecting their society (top-down).
An algorithm can be brought into any composition imagined by its creator, various
ways of how ML and ABM can work together have surfaced. Firstly, before running a
ABM, ML can derive parameter values which will serve as agent attributes [[8]](#8).
Secondly, during the execution of a ABM, ML can allow agents to learn from past
experiences and make more informed decisions via reinforcement learning
[[9]](#9), [[10]](#10), [[11]](#11).
Thirdly, ML can be used to analyse results of a ABM [[12]](#12).
Hence we can conclude, that every stage of an ABM can be set in composition with ML.

Since events such as the Cambridge Analytica scandal or Lee Sedols loss against
AlphaGo took place, ML and its relation to data is being widely discussed and
debates on the connection between computer and social science received more fuel.
Many of the breakthroughs in our understanding of the datafied society are
applicable to algorithms and data in general. However, there are stronger and
fainter nuances that pose algorithms and data differentiable. These nuances can
only be discovered and understood, by tuning the questions to each algorithm
individually. As it is my impression that simulations of societies gain in
importance, I have started to think about the following three broad themes:

1. Artificial society redefines societies agency
    - How does our participation in the decision making process change, when government policies rely ever more on outcomes of a artificial society?
    - How will an artificial society change cultural evolution differently from ML, as the prior is exerting power on an individual, that is less visible to it?
2. Malicious exploits of artificial societies
    - Will data privacy need to be extended from a individual to a society?
    - As it can be argued that any governmental attempts of evidence-based policy are hindered by its virtue to capture and control knowledge, in what circumstances do artificial societies produce policy-based evidence?
3. The current state of design and usage of standards
    - How do data analysts interpret/view data, that is gaining political sensitivity in states of emergencies?
    - What effect do the guidelines and standards have on algorithmic solution in state of emergencies? (E.g. how did the efforts of IEEE, ISO, The Open Modeling Foundation, and the Government Office for Science influence the creation of algorithmic solutions w.r.t. Covid-19)

### References
<a id="1">[1]</a>
Schelling, T. C. (1971).
Dynamic models of segregation.
Journal of Mathematical Sociology, 1(2), 143-186.

<a id="2">[2]</a>
Li, Y et al. (2016).
Agent-Based Modeling of Chronic Diseases: A Narrative Review and Future Research Directions.
Preventing Chronic Disease, 13.

<a id="3">[3]</a>
Tracy, M. et al. (2018).
Agent-based modeling in public health: current applications and future directions.
Annual Review of Public Health, 39, 77-94.

<a id="4">[4]</a>
Silverman, E. et al. (2020).
Situating Agent-Based Modelling in Population Health Research.
pre-print on arxiv:2002.02345.

<a id="5">[5]</a>
Zhan, Nan et al. (2020).
Impact of intervention methods on COVID-19 transmission in Shenzhen.
Building and environment, 180, 107106.

<a id="6">[6]</a>
Gharakhanlou, Navid Mahdizadeh and Hooshangi, Navid (2020).
Spatio-temporal simulation of the novel coronavirus (COVID-19) outbreak using the agent-based modeling approach (case study: Urmia, Iran).
Informatics in Medicine Unlocked, 20, 100403,.

<a id="7">[7]</a>
Ferguson, N. et al. (2020).
Report 9: Impact of non-pharmaceutical interventions (NPIs) to reduce COVID19 mortality and healthcare demand.

<a id="8">[8]</a>
Kavak, H. et al. (2018).
Big data, agents, and machine learning: towards a data-driven agent-based modeling approach.
In Proceedings of the Annual Simulation Symposium, 1-12.

<a id="9">[9]</a>
Taylor, Richard and Besa, M{\`o}nica Coll and Forrester, John (2016).
Agent-based modelling: A tool for addressing the complexity of environment and development policy issues.
Stockholm Environment Institute.

<a id="10">[10]</a>
Ramchandani, Pia and Paich, Mark and Rao, Anand (2017).
Incorporating Learning into Decision Making in Agent Based Models.
In EPIA Conference on Artificial Intelligence, 789-800, Springer, Cham.

<a id="11">[11]</a>
K. Brearcliffe, Dale and Crooks, Andrew (2020).
Creating Intelligent Agents: Combining Agent-Based Modeling with Machine Learning.
In The 2020 Computational Social Science Society of Americas Conference.

<a id="12">[12]</a>
Heppenstall, Alison J and Evans, Andrew J and Birkin, Mark H (2007).
Genetic algorithm optimisation of an agent-based model for simulating a retail market.
Environment and Planning B: Planning and Design, 34(6), 1051-1070.
