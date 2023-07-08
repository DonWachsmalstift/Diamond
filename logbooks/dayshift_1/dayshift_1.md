## huge delay since cryocooler malfunction
## start of alligning and measuring stuff roughly 17:00

installation of MS of I15-1:<br>
decision on measurement mode of MS: we measure 0 to 50 amu, because measurement speed is quite high and this way we may detect ethanol forming as side-product

connection of gas setup from industrial beamline to our setup

Varex detector mounted on one tip
## maximum counts allowed: 35.000 cts/per image (i.e. 3s - exposure)

Laptop for control of T ramp in server room next door makes T log file

## programming heat ramps
- saving data:<br>
 OCP-Scope $\rightarrow$ Default $\rightarrow$ Loop (Sp1 & Sp2) $\rightarrow$ Main (Working Sp) <br>
[ ] file called 2023_07_07_17:40
- Temp Ramp programming / starting:<br>
Programmer $\rightarrow$ Run $\rightarrow$ Mode $\rightarrow$ run

## instrument control software
moves sample stage in and out to predefined positions:
- sampleIn
- sampleOut

howToCheckSample
- check filters - filter is automatically determined by software from test shot and then listed in logfile
- envX: sample movement by 1 mm on x axis; there is a hard limit implemented to not crush into things

data collection
- collect_pe2['bkg', 600, frames=1: if we use bck it just measures without using sample information from
- currently 3 s integration time and we can program only multiples thereof

each data collection started creates: *.nxs, *.xy <br>
processed directory/tth_pe2: *.xy with I(2theta) 

Data Acquisition Client
- click dataset left --> click "Azimuthal Integrate [1,3841] right --> choose Plot Type "Line"

**stop running** script by going to console, click "abort all running commands", then go to tab "queue" and find most recent running script, press button on the right "stop job"

## Microreactor - Gas flow control
- software opened in another desktop
- numbers in ml/min
- MF2: He
- MF4: H2
- MF5: CO2 
Pos1 CO2 He H2<br>
Pos2 CO2 He Air

## calibration
16:49 mount of LaB6 into flow cell for setup and calibration<br>
17:12 manual alignment of sample position; no laser alignment, but green crosses on monitor.<br>
The flow cell cannot be driven in vertical direction with any motor, so no absorption can be carried out.<br>
- filenumbers #55363, #55364, #55365

## empty flow cell and empty capillary for background
**17:56**: empty sample environment
- 5 s: 55368, #55366 - 55368 have x-axis from 0 to ~35 instead of 0 to ~3500
- 60 s / 10 frames: #55369
**18:20**: empty capillary with Al-Kapton shield
- #55370: 5 frames à 120 s
**19:19**: empty capillary without Al-Kapton shield
- #55371: 5 frames à 120 s
- increase in background at ca. 31 ° 2theta corresponds to ca. 80% of Q-range; this correlates to end of triangular shaded area on left detector side
- currently 0.8 ° 2theta --> Qmin = 4pi/0.16*sin(0.4) = 0.55 A-1
- the script had f(1) as default, so all measurements before were measured with the filter, that's why data is noisy
- #55372: 4 frames à 120 s (aborted during running to access hutch), without filter

## Re-alignment and MS connection with Phil, 20:00
Beamstop is moved a bit closer, Qmin changed to ~ 0.6 A-1<br>
data integration now outputs Q<br>
cake integration of data uses only a very small cake of data (ca. 25 %), throwing away most of it<br>

## empty capillary collected again #55374

air con in room is a bit weak, so recovering the detector every now and then helps
in the detector image there are streaks above and below the beamstop --> likely shadows / parasitic scattering from the wires

## MS control software
run a scan from galery --> Bar Mode, select 1 - 100<br>
after experiment: press yellow Stop bottom<br>
export as *.csv<br>
 
## tightening capillary and validate MS functioning
empty capillary mounted, tight, gases flown through, weight signal detected in MS

