# CO2 Scrubber Bedlife Estimation

Calculations made following this Navy dive [manual](https://apps.dtic.mil/sti/tr/pdf/ADA160181.pdf). Slight modifications made to account for dead volume.

## Pre-conditions


Temperature: 

\(T=70\:F\)
{: .center-text}

Pressure at analysis depth: 

\(P_{depth}=1.6\:bar\) or \(1.5790768\:ata\)
{: .center-text}

CO2 injection rate for scrubber evaluation: 

\(rate_{CO2}=1.6\:L/min\)
{: .center-text}

Tidal lung capacity:

\(V\llap{-}_{tidal}=3\:L\)
{: .center-text}

Per breath fractional oxygen consumption in each breath (Assuming \(V\llap{-}_{in} = V\llap{-}_{out}\)): 

\(O2_{consumption\:fraction}=0.04\) 
{: .center-text}

Guppy CCR dead volume:  

\(V\llap{-}_{dead}=0.1753128081\:L\)
{: .center-text}

Fractional increase required to compensate for dead volume: 

\(V\llap{-}_{percent\:inc}=1.058437603\)
{: .center-text}


## CO2 concentration in gas stream 


Respiratory quotient: 

\(RQ=0.85\)
{: .center-text}

Pre-compensation oxygen consumption: 

\(VO2_{pre-comp}=RATE_{CO2}/RQ=1.882352941\:L/min\:at\:STPD\)
{: .center-text}

Approximate respiratory minute volume (No dead volume compensation): 

\(RMV_{pre-comp}=VO2/O2_{consumption\:fraction}=47.05882353\:L\) 
{: .center-text}

Approximate respiratory minute volume (Dead volume compensated): 

\(RMV=RMV_{pre-comp}*V\llap{-}_{percent\:inc}=49.80882836\:L\) 
{: .center-text}

Compensated oxygen consumption: 

\(VO2=RMV/24=2.075367848\:L/min\:at\:STPD\)
{: .center-text}












