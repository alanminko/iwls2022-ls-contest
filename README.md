## Problems and Results of IWLS 2022 Programming Contest

This repository contains the benchmarks of [IWLS 2022](https://www.iwls.org/iwls2022/program.php) 
Programming Contest and the circuits produced by the participants in response to the challenge.  

The goal of the contest was to synthesize [AIGs](https://en.wikipedia.org/wiki/And-inverter_graph) 
with the minimal number of two-input and-nodes, for a set of completely-specified multi-output Boolean functions 
represented using truth tables. The AIGs had to be submited in [binary AIGER format](http://fmv.jku.at/aiger/).
For the detailed information about the rules and evaluation criteria, please refer to the 
[contest description](https://github.com/alanminko/iwls2022-ls-contest/blob/main/IWLS_2022_Programming_Contest.pdf).

The contest was organized by Alan Mishchenko and Satrajit Chatterjee (IWLS 2022 Contest Chairs) 
with active support from Luca Amar? (IWLS 2022 General Chair), Eleonora Testa (IWLS 2022 Program Chair),
and Walter Lau Neto (IWLS 2022 Contest Session Chair). 

---

### Benchmarks

The [benchmarks](https://github.com/alanminko/iwls2022-ls-contest/tree/main/benchmarks) available in this repository are composed of 100 functions with truth tables listed in a text file: 

Benchnmark ID | Function Category
------------- | -----------------
00-01 | Known random-looking functions
02-07 | Random and decomposable random functions
08-09 | s-box and inverse s-box from [here](https://en.wikipedia.org/wiki/Rijndael_S-box)
10-15 | N-input [majority functions](https://en.wikipedia.org/wiki/Majority_function)
16-27 | N-input N-output [binary sorters](https://en.wikipedia.org/wiki/Sorting_network)
28-49 | Selected [Espresso benchmarks](https://ptolemy.berkeley.edu/projects/embedded/pubs/downloads/espresso/espresso-book-examples.tar.gz) with permuted inputs
50-67 | Selected arithmetic functions with permuted inputs and dropped outputs
68-99 | 12-input 3-output neurons from [LogicNets project](https://github.com/Xilinx/logicnets)

Additional details on the benchmarks are not given at this time because IWLS 2023 Programming Contest 
to be held next year may reuse the current benchmarks and/or propose similar ones.

The goal of the future contest is expected to be similar (synthesizing minimal circuits) while allowing 
for any two-input nodes (not only and-nodes, as in this year's contest).
  
A detailed description of the next year's contest (in particular, how two-input xor-nodes are saved in the AIGER format, 
which by default allows for two-input and-nodes only) will be announced later, while this preliminary announcement 
is expected to motivate future participants to plan and prepare in advance.

---

### Participants

The seven teams that participated in the contest are listed in the alphabetical order.

* **Team EPFL** (?cole Polytechnique F?d?rale de Lausanne)
  * Andrea Costamagna, Siang-Yun Lee, Alessandro Tempia Calvino, Hanyu Wang, Mingfei Yu, Professor Giovanni De Micheli
* **Team Fudan** (Fudan University, Shanghai) 
  * Yishan Zhang, Professor Chang Wu
* **Team NTU** (National Taiwan University) 
  * Hao-Ren Wang, Guo-Wei He, Professor Jie-Hong Roland Jiang
* **Team TUW** (Technische Universit?t Wien) 
  * Franz-Xaver Reichl, Friedrich Slivovsky, Stefan Szeider
* **Team UCAS** (University of Chinese Academy of Sciences) 
  * Liwei Ni
* **Team UCB** (University of California, Berkeley) 
  * Yukio Miyasaka
* **Team UFRGS/UFPEL** (Federal University of Rio Grande do Sul / Federal University of Pelotas) 
  * Jo?o Machado (UFPEL), Gabriel Ammes (UFRGS), Renato Peralta (UFRGS), Professor Andr? Reis (UFRGS), Paulo Butzen (UFRGS), Leomar da Rosa (UFPEL), Professor Renato Ribas (UFRGS)

---
       
### Submissions

With the participants' permission, the circuits submitted to the contest can be found [here](https://github.com/alanminko/iwls2022-ls-contest/tree/main/submissions).

---

### Winners

The results of the competition are summarized in the organizers' presentation 
([PDF](https://github.com/alanminko/iwls2022-ls-contest/blob/main/IWLS_2022_Contest_Presentation.pdf),
[Video](https://www.youtube.com/watch?v=BJ-72Nx9raw)).

The winners are the three teams who received the highest [resulting scores](https://github.com/alanminko/iwls2022-ls-contest/blob/main/submissions/scores.txt) according to the [contest rules](https://github.com/alanminko/iwls2022-ls-contest/blob/main/IWLS_2022_Programming_Contest.pdf):

* **1st place** (score 9388)
  * Team EPFL -- presentation [video](https://youtu.be/qUnB-01oMiQ)
* **2nd place** (score 9117)
  * Team UCB -- presentation [video](https://www.youtube.com/watch?v=tK6SVAF2gMU) 
* **3rd place** (score 8320)
  * Team TUW -- presentation [video](https://www.youtube.com/watch?v=BumyhlIKnHY) 

An honorable mention goes to **Team UFRGS/UFPEL** for synthesizing circuits with the smallest number of 
[logic levels](https://github.com/alanminko/iwls2022-ls-contest/blob/main/submissions/levels.txt). 
The logic level count was not the official competition metric, but this is nevertheless a great result.

Congratulations to the winners!

---








