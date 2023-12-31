# Memory Design

## Table of Contents

- [LTbasics](#LTbasics)
- [Inverter](#Inverter)
- [6T](#6T)
- [8/10T](#8/10T)




## LTbasics
- Understand basic analysis types in LTSpice.
- Run an inverter transient and DC analysis.
- Assignment :
	- Calculate the power of a nominally sized inverter driving a load of 1fF/5fF.
	- Calculate Fan out of 1 (FO1) and Fan out of 4 (F04) delay of the nominally sized inverter at nominal and +/-10% supply.
	- Calculate the leakage power of a 50fin inverter and compare it with a 22nm planar FET inverter of the same width.

Schematic Diagram :
- NMOS: Id vs Vgs Schematic Diagram </br>
  <img src = "LTbasics/nmos_id_vgs_l1.jpg" width="50%" height="50%"> </br>
- NMOS: Id vs Vds Schematic Diagram  </br> 
  <img src = "LTbasics/nmos_id_vds_l1.jpg" width="50%" height="50%"> </br>
- PMOS: Id vs Vgs Schematic Diagram  </br> 
  <img src = "LTbasics/pmos_id_vgs_l1.jpg" width="50%" height="50%"> </br>
- PMOS: Id vs Vds Schematic Diagram  </br> 
  <img src = "LTbasics/pmos_id_vds.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- NMOS: Id vs Vgs plots </br>
<img src = "LTbasics/op_nmos_id_vgs.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when w = 320, 640, 960, 3200, 4200n </br>
- NMOS: Id vs Vds plots </br>
<img src = "LTbasics/op_nmos_id_vds.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when Vgs = 0, 1, 2, 3, 4, 5 V </br>
- PMOS: Id vs Vgs plots </br>
<img src = "LTbasics/op_nmos_id_vgs.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when w = 320, 640, 960, 3200, 4200n </br>
- PMOS: Id vs Vds plots </br>
<img src = "LTbasics/op_pmos_id_vds.jpg" width="70%" height="70%"> </br>
Different colors showing different values of Id when Vgs = 0, 1, 2, 3, 4, 5 V </br>


## Inverter
- Run an inverter transient and DC analysis.
- Assignment :
	- Calculate the power of a nominally sized inverter driving a load of 1fF/5fF.
	- Calculate Fan out of 1 (FO1) and Fan out of 4 (F04) delay of the nominally sized inverter at nominal and +/-10% supply.
	- Calculate the leakage power of a 50fin inverter and compare it with a 22nm planar FET inverter of the same width.

Schematic Diagram :
- CMOS Inverter Schematic Diagram </br>
DC Analysis </br>
<img src = "Inverter/dc_cmos_inv.jpg" width="50%" height="50%"> </br>
AC Analysis </br>
<img src = "Inverter/ac_cmos_inv.jpg" width="50%" height="50%"> </br>
Transient Analysis </br>
<img src = "Inverter/cmos_inv.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- CMOS Inverter Waveform </br>
DC Analysis </br>
<img src = "Inverter/op_dc_cmos_inv.jpg" width="70%" height="70%"> </br>
AC Analysis </br>
<img src = "Inverter/op_ac_cmos_inv_corr.jpg" width="70%" height="70%"> </br>
Transient Analysis </br>
<img src = "Inverter/op_cmos_inv.jpg" width="70%" height="70%"> </br>
- Power Analysis </br>
Load = 1fF </br>
<img src = "Inverter/power_cmos_1f.jpg" width="70%" height="70%"> </br>
Total Power consumed by CMOS Inverter = 201.78 μW (PMOS) + 202.57 μW (NMOS) </br>
Load = 5fF </br>
<img src = "Inverter/power_cmos_5f.jpg" width="70%" height="70%"> </br>
Total Power consumed by CMOS Inverter = 202.57 μW (PMOS) + 202.83 μW (NMOS) </br>


## 6T
- Desing and Analysis of 6T SRAM Cell.
- Perform Static-noise margin analysis of the same refer to this ["Static-noise margin analysis of MOS SRAM cells"](https://ieeexplore.ieee.org/document/1052809) 

Schematic Diagram :
- Transient Analysis of 6T SRAM Cell </br>
<img src = "6T/sram_6t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "6T/sram_6t_snm.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- Transient Analysis of 6T SRAM Cell </br>
<img src = "6T/op_Sram_6t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "6T/op_sram6t_snm_1.jpg" width="70%" height="70%"> </br>
<img src = "6T/op_sram6t_snm_2.jpg" width="70%" height="70%"> </br>
<img src = "6T/op_sram6t_snm_3.jpg" width="70%" height="70%"> </br>


## 8/10T
- Desing and Analysis of 8T and 10T SRAM Cell.
- Perform Static-noise margin analysis of the same refer to this ["Static-noise margin analysis of MOS SRAM cells"](https://ieeexplore.ieee.org/document/1052809) 

Schematic Diagram :
- Transient Analysis of 8T SRAM Cell </br>
<img src = "8_10T/sram_8t/sram_8t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 6T SRAM Cell </br>
<img src = "8_10T/sram_8t/sram8t_snm.jpg" width="50%" height="50%"> </br>

- Transient Analysis of 10T SRAM Cell </br>
<img src = "8_10T/sram_10t/sram_10t.jpg" width="50%" height="50%"> </br>
- Static-noise margin analysis of 10T SRAM Cell </br>
<img src = "8_10T/sram_10t/sram10t_snm.jpg" width="50%" height="50%"> </br>

Resultant Waveform :
- Transient Analysis of 8T SRAM Cell </br>
<img src = "8_10T/sram_8t/op_sram8t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 8T SRAM Cell </br>
<img src = "8_10T/sram_8t/op_sram8t_snm.jpg" width="70%" height="70%"> </br>
<img src = "8_10T/sram_8t/op_sram8t_snm_1.jpg" width="70%" height="70%"> </br>
<img src = "8_10T/sram_8t/op_sram8t_snm_2.jpg" width="70%" height="70%"> </br>

- Transient Analysis of 10T SRAM Cell </br>
<img src = "8_10T/sram_10t/op_sram10t.jpg" width="70%" height="70%"> </br>
- Static-noise margin analysis of 10T SRAM Cell </br>
<img src = "8_10T/sram_10t/op_sram10t_snm_1_1.jpg" width="70%" height="70%"> </br>
<img src = "8_10T/sram_10t/op_sram_10t_snm_2_1.jpg" width="70%" height="70%"> </br>
<img src = "8_10T/sram_10t/op_sram10t_snm_3.jpg" width="70%" height="70%"> </br>

