---
{"dg-publish":true,"permalink":"/01-nthu/ee/electronic/small-signal-model/","title":"Small Signal Model","tags":["NTHU/EE/Electronic"]}
---

# MOS
![Pasted image 20240616134828.png](/img/user/Image%20Source/Pasted%20image%2020240616134828.png)
- Transconductance: 
$$
g_m = \mu C_{ox} \frac{W}{L} (V_{GS}-V_{TH}) = \sqrt{2I_D\mu C_{ox}\frac{W}{L}} = \frac{2I_D}{V_{GS}-V_{TH}}
$$
- output impedence: 
$$
r_0 = \frac{1}{\lambda I_D}
$$
- input impedence: $\infty$

# BJT
![Pasted image 20240616134930.png](/img/user/Image%20Source/Pasted%20image%2020240616134930.png)
- Transconductance: 
$$
g_m = \frac{dI_c}{dV_{BE}} = \frac{I_c}{V_T}
$$
- input impedence:
$$
r_{\pi} = \frac{dV_{BE}}{dI_B} = \frac{\beta}{g_m} = \frac{V_T}{I_C}
$$
- output impedence 
$$
r_d = \frac{dV_CE}{dI_C} = \frac{V_A}{I_C}
$$
