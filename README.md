HAP1_rRNA_fraction1_rep1.mzML  
HAP1_rRNA_fraction1_rep2.mzML  
HAP1_rRNA_fraction1_rep3.mzML  
HAP1_rRNA_fraction2_rep1.mzML  
HAP1_rRNA_fraction2_rep2.mzML  
HAP1_rRNA_fraction2_rep3.mzML

Детекция пиков по MS1 (centroided)

Для каждого скана MS1 считались пики с m/z и интенсивностью.

Пики с интенсивностью ниже верхнего 1% (percentile = 99) отбрасывались, чтобы уменьшить шум и ускорить обработку.

Группировка и объединение данных

Пики, близкие по m/z (±0.0001) и RT (±0.01 мин), объединялись.

Для каждого пика суммировалась интенсивность и перечислялись файлы, в которых он встречался.


<img width="1022" height="540" alt="Снимок экрана 2026-02-15 в 17 25 31" src="https://github.com/user-attachments/assets/9dcdce33-fc81-4a89-b7e5-40f094d81c54" />
