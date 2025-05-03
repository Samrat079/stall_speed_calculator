<p align="left">
    <img src="favicon.svg" alt="AeroCal logo" width="120"/>
</p>    

<h1 align="Center"><strong>AeroCal</strong>

# ✈️ Stall Speed Calculator

**Overview**

AeroCal introduces simple and clean stall speed calculator accessable through your browser. Most aerodynamic calculation including stall speed of an aerofoil has been quite difficult as the information required to calculate said value like wing area, weight, cofficient of lift etc. are confidential in both military and commertial applications. 

Thus we have made a calculator which is able to performe calculations of similler accuracy to the original version but with values which are easer to come by or are easier to estimate using publically avalable data. Stall speed can be calculated by using wing loading, altitude and CLMax. We have also we have also modified the formula where it can use the above mentioned variables more on the formula below.

## 🌐 Live Demo

[Visit here](samrat079.github.io/stall_speed_calculator/)

## ⚙️ How Does It Work?

### 🧪 Traditional Formula

**Vs** = √(2 * W / (ρ × S × CL))

Where:  
- **Vs** = Stall speed  
- **W** = Aircraft weight  
- **ρ** = Air density  
- **S** = Wing area  
- **CL** = Maximum lift coefficient

As it is apperant that the information like wing area, air density etc requir ether deeper knowledge into the design or the air craft or about aerodynamics to make an educated guess. 

The alternative formula that we have come up with makes this calculation a little easier by incormorating the pressure and altitude calculation within the formula and also the simplifing the weight, lift and wing area into wing loading. 

### 🧮 Our Simplified (and Cooler) Formula

**Vs= √[ (2 × WL × 9.80665) / (CLₘₐₓ × (101325 × (1 − (0.0065 × h × 0.3048) / 288.15)^5.25588)) ] × 1.94384

Where:
- **Vs** = Stall speed in **knots**
- **WL** = Wing loading in **kg/m²**
- **CLₘₐₓ** = Maximum lift coefficient 
- **h** = Altitude in **feet**

As you can see this formula looks much more intimidating but it only has 4 variables, actually 3 Vs is the answer. This formula allows you to add just these 3 values and it gives you the answer. 

## ⚠️ Limitations

There are some limitations to this way of finding stall speed, this formula is made to only work with metric units using imperial requires to perform a unit conversion(Avalable on the site) also if you want to find the stall speed of an aerofoil which is going to work underwater or in diffrent planet with diffrent atmosphere its not going to work. Although i suppose a calculation within the earths atmosphere is what is needed for the time being. 

**📦 Want to run locally?**

```bash
git clone samrat079.github.io/stall_speed_calculator/
cd stall-speed-calculator
open index.html
