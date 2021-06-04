
EC based fan control (I may send a PR to smcsuperio)  
Register 0x16 (21) --> Manual fan control. This resets after a sleep/wake cycle  
Options:  
- 0x0 (Disabled)
- 0x1 (Manual fan control)

Register 0x1A (25) --> Fan speed   

Speeds:  
55  
54  
53 (Used by EC, so skip this value if you want to linearly ramp up the fan)  
52  
51  
50  
49  
48  
47 (Used by EC, so skip this value if you want to linearly ramp up the fan)  
46   
45  
44  
43 (Used by EC, so skip this value if you want to linearly ramp up the fan)  
42  
41  
40  
39  
38 (Used by EC, so skip this value if you want to linearly ramp up the fan)  
37  
36  
35  
34  
33  
32  
31 (Used by EC, so skip this value if you want to linearly ramp up the fan)    
30  
29  
28  
27  
26 (Used by EC, so skip this value if you want to linearly ramp up the fan)
25  
24  
23  
22  
21  
20  
19  
18   
17  
16  
15  
14  
13  
12   
11  
10   
9  
8  
7  
6  
5  
4  
3  
2  

If you play around with this, you will get what I mean.
