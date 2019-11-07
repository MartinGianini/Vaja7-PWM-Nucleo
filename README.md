2.)
b)pin PA8, TIM1_CH1
d)16
e)10Khz
f)širina pulza, 50% = kvadratni pulz (na osciloskopu)


3.)
c)sConfigOC.Pulse = 50;


5.)
a)sConfigOC.Pulse = 25;

"c")
1-vrednost zanke htim1.Istance->CCR1 postane vrednost dutyCycle-a
2-širina se poveča za 10% 
3-če pulz preseže 90%, se postavi nazaj na 10%


Delovanje:
V CubeMX-u nastavljeni parametri, ter koda na osclioskopu prikaže nespremenljiv štirioglat sinus pri 1Mhz, po navodilih do nal. 4 pri 50% pulzu.
Po navodilih iz nal. 5 je pulz 25% in se širi za 10%. Ko pulz preseže 90%, se skrči nazaj na 10% in ponovi cikel.
