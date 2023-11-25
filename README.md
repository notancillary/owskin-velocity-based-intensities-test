# owskin-velocity-based-intensities-test
Test to determine the feasibility of utilizing velocities to determine intensity. <br>
<br>
Create empty on spine bone with a contact reciever a bit larger than your torso overall
<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/3df37e6c-000f-46f8-bec1-c9f8c201bfe2)
<br><br>
set the standard collision tags <br>
use the param low_vel_1 <br>
set to 0.1 min vel on enter <br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/55e4b84d-21b8-40fe-ad4d-92a7bf6a2134)
<br>
<br>
copy that contact reciever script twice with the following parameters and velocities
<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/0ca1a2c8-a8c5-419d-8288-2927b422916f)
<br><br>
add them to your fx as bools
<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/4578738c-501d-470f-aac1-3381259cbce7)
<br><br>
create this state machine in a new layer... (dont forget to set the layer weight to 1) 
<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/4a6b69fb-6c40-43fe-beac-3bbc28b75adf)
<br><br>
transition for low is<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/9d0b0f49-0b38-4ece-8670-2aef6581913d)
<br><br>
med<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/d976884f-9fda-46a3-bac9-4516004809e5)
<br><br>
high<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/fd08511b-34c0-41a9-8599-98b27f7854ca)
<br><br>
declare the owo_intensity parameter in your avatar parameter list..<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/d4d389be-7d8d-4fd7-890c-e670e7552283)
<br>
<br>
using a avatar parameter driver i set low to 0.5, med to .75 and high to 1<br>
![image](https://github.com/notancillary/owskin-velocity-based-intensities-test/assets/50598087/47e81154-4772-4e8b-b158-400b83d3b48e)
<br><br>
You need to use version 0.0.7 for this to work: <br>
https://github.com/uzair-ashraf/vrc-owo-suit/releases/tag/0.0.7<br>
<br>

Note that this is a test to determine if this sort of interaction is beneficial/ideal. Preliminary testing points to yes. This will ultimately be implimented with infinitely scaling intensities, instead of these 3 stages.. but this gets you 80% of the way there if you want to try it now. Additional updates will add auto-detection of specific sensations.. <br>
