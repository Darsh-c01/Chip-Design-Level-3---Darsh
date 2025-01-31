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








