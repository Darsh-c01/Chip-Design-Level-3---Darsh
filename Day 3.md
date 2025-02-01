# <ins> Day 3 -> Labs for CMOS inverter ngspice characteristics </ins>
## Changing IO properties

OpenLANE has the feature of changing things on the fly by using the command:
>set variablename value

We can do this for the IO pins as mentioned in the video.

## LABS
### Image sources : My device
First we take the files from the repo shared in the video and use the git clone command for it.
![image](https://github.com/user-attachments/assets/37f08c6e-8d48-45e4-b07f-333a8587e6ff)
![image](https://github.com/user-attachments/assets/35a1e79a-04ff-4c4c-9791-cfaf96c8ca76)
Now we can see there is a new folder created. \

Next what we do is we move the sky130A.tech file into the directory wich just got created using the copy command.
![image](https://github.com/user-attachments/assets/06a4f62c-f3f9-4687-bd4b-2e3fd9ec3310)

Next we open the command on Magic , using a simillar command is earlier 
>magic -T

![image](https://github.com/user-attachments/assets/a95da08a-5d17-4d24-a80d-f618c6300af7)
The output of this is as follows 
![image](https://github.com/user-attachments/assets/594a862a-76a5-49ea-9165-2e71c7862b36)
>We can notice in this image some colours to the right , these are basically the different layers.

#### Checking the NMOS and PMOS 
##### 1.NMOS
![image](https://github.com/user-attachments/assets/e9b084a0-e6b0-42d4-9071-4ba97eae633c)
##### 2.PMOS
![image](https://github.com/user-attachments/assets/54334217-6e92-462c-b397-d365c580e7be)

### Extracting the SPICE file:
First in the Tkcon window , we run the command extract
![image](https://github.com/user-attachments/assets/46f1423e-467e-4680-9ea1-b42a03c9b5e7)
This leads to the creation of a new file which can be seen in the following image:
![image](https://github.com/user-attachments/assets/1ac095da-d8a3-4b91-bbc3-b720d7383e5a)

<ins> Next we create the SPICE file </ins>
![image](https://github.com/user-attachments/assets/def9a2b3-1ab0-4d00-b1df-9f0417484f83)
We can now see this file below
![image](https://github.com/user-attachments/assets/ffca9411-90a4-44c0-9082-f4044bb74034)

Interior of the SPICE file 
![image](https://github.com/user-attachments/assets/768e237b-963b-4b67-947f-e8285930c877)

Next we edit the spice file as below
![image](https://github.com/user-attachments/assets/f6b644b8-9d71-4fb6-a499-303a42f877bd)

















