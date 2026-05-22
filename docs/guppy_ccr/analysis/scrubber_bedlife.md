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


## Scrubber dimensions

Axial scrubber length:

\(L_{canister}=0.62\:ft\)
{: .center-text}

Axial scrubber diameter:

\(D_{canister}=0.31\:ft\)
{: .center-text}

Axial scrubber length to diameter ratio:

\(L/D=2\)
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

Compensated oxygen consumption (See manual for formula): 

\(VO2=RMV/24=2.075367848\:L/min\:at\:STPD\)
{: .center-text}

Volumetric flow rate to canister:

\(   Q=RMV/28.3168\:L/ft^3=1.758985068\: ft^3/min\)
{: .center-text}

Fraction CO2 concentration in gas stream:

(Would be 1/ata instead of unitless without considering that the numerator is measured assuming STPD conditions)

\(CO2_{fraction}=(VO2*RQ/Q*P_{depth})/28.3168\:L/ft^3=0.022428717\)
{: .center-text}

CO2 percentage concentration in gas stream:

\(CO2_{\%}=CO2_{fraction}*100=2.2428717\%\)
{: .center-text}


## Surface Level Equivalent

Surface level equivalent CO2 concentration percentage:

\(CO2_{\%\:SLE}=CO2_{\%}*P_{depth}=3.541666667\%\)
{: .center-text}


## Bulk density of absorbent

Sofnolime 797 CO2 Absorbent (Provided by manufacture):

\(\varphi_{absorbent}=0.9\:g/cm^3\)
{: .center-text}

## Absorbent weight

Scrubber canister volume:

\(V\llap{-}_{scrubber\:canister}=\pi*(D_{canister}/2)^2*L_{canister}*1728\:in^3/ft^3=80.86278535\:in^3\)
{: .center-text}

Absorbent weight:

\(W_{absorbent}=V\llap{-}_{scrubber\:canister}*\varphi_{absorbent}*16.3871\:cm^3/in^3*0.00220462\:lbm/g=2.629220762\:lbm\)
{: .center-text}

## Density of CO2 at operating pressure

CO2 molecular weight:

\(M_{CO2}=44.01\:lbm/lbm\text{-}mole\)
{: .center-text}

Pressure absolute:

\(P_{abs}=P_{depth}*14.6959\:lbf/in^2/ata=23.20595475\:lbf/in^2\)
{: .center-text}

Universal gas constant:

\(R=1544\:ft\:lbf/lb\text{-}mole*\,^{\circ}\text{R}\)
{: .center-text}

Temperature (Rankine):

\(T_{R}=T+459.67=529.67\,^{\circ}\text{R}\)
{: .center-text}


Density of CO2 at operating pressure:

\(\varphi_{CO2}=(M_{CO2}*P_{abs}/R*T_{R})*144\:in^2/ft^2=0.179829373\:lbm/ft^3\)
{: .center-text}


## Absorbent capacity 
Data used for this calculation is taken from [this](https://www.divegearexpress.com/amfile/file/download/file/76) Sofnolime 797 laboratory report.  

All abbreviations used in this section are local context only.

Ambient pressure during test:

\(P_{test}=3\:bar\)
{: .center-text}

Measured average absorbent capacity:

\(Absorbent_{cap}=107L(CO2)/kg(Sofnolime)\)
{: .center-text}

Mass of absorbent used:

\(M_{absorbent}=1kg\)
{: .center-text}

Temperature:

\(T_{test}=277.15K\)
{: .center-text}

Ideal gas constant:

\(R = 0.08314462618\:L*bar/K*mol\)
{: .center-text}

Volume of CO2:

\(V\llap{-}_{CO2}=107L\)
{: .center-text}

Van der Waals number of moles calculation:

\(   \)