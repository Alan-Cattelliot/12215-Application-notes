# 12.7 Combination of diagonal load LC1 and rig load LC2 for sailing multihulls

## Additionnal notes from HDS report
*march 2015*, @R.Balze, @A. Miler, @R. Vicariot

1. References 
2. Definition of loads 
3. Materials
4. Dynamic and safety coefficients 
5. Calculation of GLC1 : Diagonal swell 
6. Calculation of GLC2 : Rigging forces 
7. Max stress 
8. Conclusion ANNEXES A and B : Calculation of equivalent stiffnesses

## 1. References 
`[1]` WG 18 N 328 rev4 DIS2 12215-7-2012-11-09 Pre Mets
`[2]` ISO 12215-5 F-2008

## 2. Definition of loads
According to paragraph `12.1.3` in `[1]`, the loading applied to the beams is as follows : 

<img src="https://render.githubusercontent.com/render/math?math=max \{ \frac{1}{2} GLC_{1} %2B GLC_{2}, GLC_{1} %2B \frac{1}{2} GLC_{2} \}">

With :
GLC1: Diagonal swell 
GLC2: Rigging forces 

The fore and aft beams will be analysed under this loading case. 
The "K method" detailed below __applies only to the aft beam__.

## 3. Materials
The material characteristics are defined as presented in `[2]`.

## 4. Dynamic and safety coefficients
- GLC1 : Dynamic coefficient nCGMH present in the calculation of the torsional moment of the MTDplatform (see `[1]`).

- GLC2 : Dynamic factor nCGMH applied to the rigging forces (see `[1]`).

The safety coefficients to be applied to the failure stress of the materials are detailed in paragraph `12.2` of `[1]`.in paragraph '12.2' of `[1]`.
Example: For FRP <img src="https://render.githubusercontent.com/render/math?math=\alpha_{materiau} = 2.0">

 

## 5. Calculation of GLC1 : Diagonal swell
The calculations of the bending moment and shear force along the beam due to GLC1 are defined in Annex C of `[1]`, equation `(C.6)` and `(C.7)` respectively. 
The calculations of the equivalent stiffnesses of beams and floats are detailed in Annexes `A` and `B` of this document. 
In order to simplify the calculations, the torsional stiffness of the beams used in equation `(C.4)` is assumed to be zero. 

![Github](GLC1_bending_moment.png)
 
 
## 6. Calculation of GLC2 : Rigging forces
### 6.1. Shear force current standard
Maximum shear force to be considered along the whole beam:

- Front beam : Mast toe compression * dynamic factor nCGMH 
- Aft boom: mainsheet force * dynamic coefficient nCGMH 

The "K method" has no influence on the shear force proposed by the standard

### 6.2. Bending moment current standard 
According to paragraph 14.2.1 in [1], the bending moment considered along the beam is :

<img src="https://render.githubusercontent.com/render/math?math=M_{fGLC2}(y) = max \{ M{fixed}(y), M{supported}(y) \}, \forall y \in [0,\frac{B_{BH}}{2}]">
<img src="https://render.githubusercontent.com/render/math?math=M_{fixed}(y) = \frac{F}{2} ( \frac{B_{BH}}{4} - y )">
<img src="https://render.githubusercontent.com/render/math?math=M_{supported}(y) = \frac{F}{2} ( \frac{B_{CB}}{2} - y )">

![Github](GLC2_fixed_aft.png)

### 6.3. Bending moment ???k method???
__Reminder: The "K method" applies only to the aft beam__ 
The considered bending moment given by the "k method" is :

<img src="https://render.githubusercontent.com/render/math?math=k = \frac{\frac{B_{CB}}{2}}{\frac{B_{CB}}{2}+\frac{L}{R_{tors}}+\frac{B_{CB}}{2R_{flex}}}">

## 7. Max stress
### 7.1. Due to shear force 
It is checked that the maximum shear stresses are less than the allowable stress of the material at 3 levels y = 0; BBH/4; BBH/2 :

With: ?????????????????????? = ?????????? ???????????????????? (For ????????????????????cf point 4.) S(y) = Cross-sectional area taking the shear (Bi-bias) ??(??) = max { 0.5* ????????1(??) + 0.5* ????????2(??); ????????1(??) } (Shear force considered) 

If this equation is verified at these 3 points, then the catamaran beams meet the standard in the Bi-biases.

### 7.2. Due to bending moment 

It is checked that the maximum normal tensile and compressive stresses are less than the allowable stress of the material at 3 levels y = 0; BBH/4; BBH/2 

With: ?????????????????????? = ?????????? ???????????????????? (For ????????????????????cf point 4. ) v: Vertical distance between the neutral fibre and the UD fibres furthest from the neutral fibre ????(??) = max {0.5* ???? ??????1(??) + ???? ??????2(??); ???? ??????1(??) + 0.5* ???? ??????2(??) } 
If this equation is verified at these 3 points, then the catamaran beams meet the norm in the UDs. 


## 8. Conclusion ANNEXES A and B : Calculation of equivalent stiffnesses
This document summarises the methods of calculating the bending beams made by the standard and by the "k method".

For each of the existing catamarans, the two methods of calculating the GLC2 (current standard and the HDS "k method") will be applied in order to account for the gains brought about by the k method. 

The results obtained will show whether the existing and proven boats can pass the standard or whether these global loads need to be refined.

