# <ins> Day 2 --> good floorplan vs bad floorplan and introduction to library cells </ins>
## Defining the Width and Height of the core and die:
### Image source - VSDIAT

The dimensions of the chip depend on the dimensions of the logic gates.  \
Lets take the following example (Images from lecture )
![image](https://github.com/user-attachments/assets/58852ca9-f767-4806-b967-e85e5be670c1)

The minimum area of this netlist is:
![image](https://github.com/user-attachments/assets/683c4d95-1a17-42ed-94a9-5fa34bfd6c8b)

Now if we place this in the core , we get the following
![image](https://github.com/user-attachments/assets/5a25f524-6ce0-44d3-a22d-32a1a35b6ea1) \
We can notice that it says the utilization is 100% , this depends on the utilization factor. 
>Utilization Factor = Area of the Netlist / Area of the core

In this case the utilization factor is 1 \
Usually the utilisation is around 50-60% 

<ins> What is Aspect Ratio ? </ins> 
>Aspect Ratio = Height / Width

Thus when the aspect ratio is 1 we can conclude that the chip is square !

## <ins> Preplaced Cells </ins>
### Image source - VSDIAT

If we look at the following image we can see that a combinational logic can actually be split into 2 parts.
![image](https://github.com/user-attachments/assets/2d9fe7e5-7c58-479f-855d-9ba0c770dc5b)

Now lets extend the IO pins and then black box. After that we will separate the 2 blocks and it will look as follows:
![image](https://github.com/user-attachments/assets/1796e415-2b24-4ad4-8649-22935f7b8ab5)

Doing this helps us reuse these models in a chip. \
That way these cells are just being implemented once and can be instentiated multiple times.

The arangement of these cells / IPs is known as <ins> floorplanning </ins> \
These cells have a pre defined location and are known as <ins> preplaced cells </ins> , they are not moved by any of the automated placement tools. 

## Defining Location of Preplaced cells:
>We place the preplaced cells based on the design senario. \
>For example , if they are connected mostly to input pins , then they will be closer to the input side of the chip.

### Next we need to surround these preplaced cells with <ins> Decoupling Capacitors </ins >

#### Noise Margin Summary 
> Lets say we want to switch from logic 0 to logic 1 , now this requires some current. \
What the <ins> Noise Margin Summary </ins>  does is, it shows us the required current for logic 0 and logic 1 , now if the current is in the gray area , then it is a problem.

![image](https://github.com/user-attachments/assets/f62c9432-f372-4cc1-84fb-5da5915de621)

If this required current comes via a source throug wires , then there will be a loss in voltage and it might go into the grey area. \
To solve this problem we use "<ins> Decoupling Capacitors </ins> "\

What is a Decoupling Capacitor ? 
> It is a huge capacitor filled with charge.

Decoupling Capacitors will be placed close to the cells and minimises the loss of voltage. Thus they are used near the cells.

### <ins> Power Planning </ins>

These days we use multiple power supplies instead of 1 so that the cells can tap in the power form the nearest power supply , this way there is also no need to have decoupling capacitors every where.

![image](https://github.com/user-attachments/assets/cf1df766-d84d-4bb4-ab1e-ad6027e0ca55)

















