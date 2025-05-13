---
{"dg-publish":true,"permalink":"/01-nthu/ee/electronic/bjt/","title":"BJT","tags":["NTHU/EE/Electronic","NTHU"]}
---

# BJT Summary
![Pasted image 20240616133948.png](/img/user/Image%20Source/Pasted%20image%2020240616133948.png)

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/01-nthu/ee/electronic/small-signal-model/#bjt" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# BJT
![Pasted image 20240616134930.png](/img/user/Image%20Source/Pasted%20image%2020240616134930.png)
- Transconductance: 
$
g_m = \frac{dI_c}{dV_{BE}} = \frac{I_c}{V_T}
$
- input impedence:
$
r_{\pi} = \frac{dV_{BE}}{dI_B} = \frac{\beta}{g_m} = \frac{V_T}{I_C}
$
- output impedence 
$
r_d = \frac{dV_CE}{dI_C} = \frac{V_A}{I_C}
$


</div></div>


# Amplifier

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




# Common Emitter 
![Pasted image 20240616115902.png](/img/user/Image%20Source/Pasted%20image%2020240616115902.png)
> Inverting Amplifier
## Small Signal Model 
- output impedence:  RC // ro
- Voltage gani : gm(RC//ro)

# Degeneration 
With another resistor at button of the device. This resistor can be used to control **voltage gain** and **output impedence**. 
![Pasted image 20240616120547.png](/img/user/Image%20Source/Pasted%20image%2020240616120547.png)

## Small Signal Model 
![Pasted image 20240616120728.png](/img/user/Image%20Source/Pasted%20image%2020240616120728.png)
這個模型的resister接在collector端，可以想像兩邊的電流都匯流到collector上面，因此流到上面的電流量將會是(base的current會是i，流往emitter會是放大$\beta$倍的電流)，所以加總起來流經collector端的電流會是$(1+\beta)$倍的電流

- Voltage gain(A_V):
$
\frac{-g_mR_C}{1+g_mR_E}
$
- input impedence: 
$
r_\pi+ (1+\beta)R_E
$
- output impedence: 
$
r_o[1+g_m(R_E//r_\pi)]
$



</div></div>



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




# Common Base
The input is at emitter side. (non-inverting amplifier)
- Very useful current buffer (current gain is close to 1)
![Pasted image 20240616132617.png](/img/user/Image%20Source/Pasted%20image%2020240616132617.png)
- Voltage Gain: 
$
g_m (R_c//r_o)
$
- Input impedence: 
$
\frac{1}{g_m}//r_\pi
$
> Take $r_o$ into consideration:
> $
\frac1{g_m} +\frac{R_C}{g_mr_o}
 $

- Output impedence: 
$
R_C//r_o 
$
## Current Buffer
Since the input is at collector side, and the output is at emitter side, the current gain is $\frac{\beta}{1+\beta}$



</div></div>



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




# Common Collector
- non-inverting amplifier
- Can be designed as voltage buffer. (emitter follower, voltage follower)
![Pasted image 20240616133327.png](/img/user/Image%20Source/Pasted%20image%2020240616133327.png)
![Pasted image 20240616133423.png](/img/user/Image%20Source/Pasted%20image%2020240616133423.png)
- Voltage Gain(AV) 
$
\frac{g_m (R_E//r_o)}{1+g_m(R_E//r_o)}
$
- Input Impedence: 
$
r_\pi +(1+\beta)(R_E//r_o)
$
- Output Impedence: 
$
\frac{1}{g_m}//r_\pi//R_E
$

![Pasted image 20240616133814.png](/img/user/Image%20Source/Pasted%20image%2020240616133814.png)

</div></div>
