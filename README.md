# Dispersion-Limited-Fiber-Length
Dispersion Limited Fiber Length
# Objective: 
 
Calculate the dispersion-limited fiber length for a fiber optic transport system that 
employs standard single-mode fiber and a directly-modulated single-mode laser diode 
transmitter. 
 
Simulate the resulting system and verify that it meets performance objective.  
 
# Theory: 
 
The maximum allowable dispersion (or pulse spread) <img width="76" height="52" alt="image" src="https://github.com/user-attachments/assets/52dff457-e7aa-4312-aef4-aa4e234afb47" /> is given in terms of the transmission rate R by the following engineering guideline <img width="192" height="124" alt="image" src="https://github.com/user-attachments/assets/4fcb3de9-6a4a-48db-ba5f-f020a6c85d8b" /> This guideline provides reasonable assurance that there will be no significant inter
symbol interference (ISI) due to pulse spread. 
 
For standard single-mode fiber driven by a directly-modulated laser diode transmitter, the 
pulse spread due to chromatic dispersion is given by
<img width="898" height="694" alt="image" src="https://github.com/user-attachments/assets/5499f4b0-2405-4a5f-b773-ce004a76e850" />
<img width="1300" height="974" alt="image" src="https://github.com/user-attachments/assets/bbd90891-43d6-4a5d-92d2-73ed3e4e57eb" />
# Layout: 
Open up the OptiPerformer file called “Dispersion Limited Fiber.osp”. This layout uses 
the Laser Rate Equations laser diode component with default parameters.  It models a 
directly modulated laser diode based using a standard rate equation model. One of the 
effects of this model is that it generates a signal with a spectral width of about 0.6 nm for 
the default parameters with 2.5 Gb/s, return to zero modulation. 
Within the layout, there are several “Visualizers.” The “Optical Time Domain 
Visualizers” allow the user to the view the simulated signal as a function of time. There is 
one at the output of the laser and one at the end of the fiber.  This allows the user to 
directly observe the changes in the pulses due fiber dispersion. The “Optical Spectrum 
Analyzer” allows the user to view the spectral content of the signal. It this lab it is used to 
verify that the spectral width is about 6 nm. The “BER analyzer” provides calculations of 
the Q factor, the bit error rate (BER) and provides a plot of the eye diagram. 
# Simulation:  
Set the laser power such to achieve a transmitter output power of 0 dBm. The transmitter 
power can be viewed by double clicking the “Output Power Meter Visualizer.” The 
power will read -100 dBm until the first run is made.  
Using the chromatic dispersion factor equation, determine the dispersion of the fiber at 
1550 nm and set the fiber dispersion parameter accordingly. 
Using the equations above, determine the dispersion-limited fiber length. 
<img width="1262" height="1044" alt="image" src="https://github.com/user-attachments/assets/e0b20ca6-42b4-4f1b-ac9a-e4f931a85001" />
# Tabulation

<img width="1010" height="1600" alt="image" src="https://github.com/user-attachments/assets/74463c3d-1106-4103-829c-018d5e1cdc74" />

<img width="1600" height="979" alt="image" src="https://github.com/user-attachments/assets/49a366cd-0412-49e1-9c93-622e7bd39896" />

<img width="1920" height="1080" alt="op exp3-1" src="https://github.com/user-attachments/assets/4c0efd76-a1b8-4d04-9729-75512c897ef6" />

<img width="1920" height="1080" alt="op exp3-2" src="https://github.com/user-attachments/assets/bcf89a38-f7ba-4313-8491-797f3de61420" />

<img width="1920" height="1080" alt="op exp3-3" src="https://github.com/user-attachments/assets/70c7ead3-7da4-4cac-9f3d-ce922e0b667e" />

<img width="1920" height="1080" alt="op exp3-4" src="https://github.com/user-attachments/assets/bb038b8c-6d01-4262-85aa-b756556e6da8" />


<img width="1920" height="1080" alt="op exp3-5" src="https://github.com/user-attachments/assets/e06b587f-42ac-4061-b3fc-d5889f7d9332" />


# Result

The dispersion-limited fiber length for the given optical communication system was found to be approximately 10 km. The simulation results showed acceptable BER performance with a clear eye diagram and minimal intersymbol interference. Hence, the system operated successfully within the dispersion limit.
