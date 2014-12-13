Why and How to Use Pseudocode
=============================

Authors
---------
Tiffany Glenn-Hall

Oscar Gonzalez

Why use pseudocode?
-------------------
Pseudocode may sound like a generic concept, but you can think of it as an outline of your code. Just like an outline of an essay/research paper you may start out with a simple outline (example one). You also need to consider the flow of information and move paragraphs around to create the best story (second example). As the essay development continues your outline fills in and you ultimately end up with a just a few points of concern (third example). Eventually everything comes together and you have a complete essay (see the function program).

What are some advantages of pseudocode?
<ol>
  <li>Explain your code to non-programmers</li>
  <li>Use it as a way of determining objects in your code (help with OOP)</li>
  <li>Use it to determine the best logic for your code</li>
  <li>Communicate your ideas to gain opinions/suggestions from other programmers</li>
</ol>


Examples of pseudocode and when to use them
-------------------------------------------


NOTES:
How do I add code to md?

How can I add more structure?

How do I add video of my programs output?

```C++
#include <stdio.h>
#include <stdlib.h> 
#include <math.h> 
#include <map>

using namespace std;

#define   ncellType1	1   
#define   ncellType2	1
#define   iters		3000
#define	  g_ampa_CT1CT2 0.00068
#define	  g_ampa_CT2CT1 0.00068
#define   g_ampa_CT1DCpulse 1.0
#define   range_left	500
#define   range_right	1000
#define   dc_amplitude	0.1
#define	  a_sin		0.4
#define   sin_bx	0.076
#define	  trial		10

const int trials[trial] = {0,5000,10000,15000,20000,25000,30000,35000,40000,45000};

//-- Regular spiking neuron---------------------------------------
class RS{
  double y, xp, xpp, sigma_n, beta_n;
public:
  double alpha, x;	
  double sigma, sigma_e, beta_e, S_CX_DEND, mu;
  int spike;	

  RS(){ init(); }

  void init(){
    spike=0;
    mu=0.0005;		
    alpha=3.65; 	
    sigma=0.06;	
    sigma_e=1.0;
    beta_e=0.03;
    S_CX_DEND = 165.0e-6;

    //initial conditions
    xpp=-1+sigma;
    xp=-1+sigma;
    x=-1+sigma;
    y= x - alpha/(1-x);
  }
  inline void calc(double);
};

```
