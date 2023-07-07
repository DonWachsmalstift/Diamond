# huge delay since cryocooler malfunction
## start of alligning and measuring stuff roughly 17:00

installation of MS of I15-1
- decision on measurement mode of MS: we measure 0 to 50 amu, because measurement speed is quite high and this way we may detect ethanol forming as side-product
- 

connection of gas setup from industrial beamline to our setup

Varex detector mounted on one tip
## maximum counts allowed: 35.000 cts/per image (i.e. 3s - exposure)

Laptop for control of T ramp in server room next door makes T log file


## programming heat ramps


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

each data collection started: *.nxs, *.xy
processed directory/tth_pe2: *.xy with I(2theta) 

Data Acquisition Client
- click dataset left --> click "Azimuthal Integrate [1,3841] right --> choose Plot Type "Line"


# Microreactor flow control
- software opened in another desktop
- numbers in ml/min
- MF2: He
- MF4: H2
- MF5: CO2 

## calibration
16:49 mount of LaB6 into flow cell for setup and calibration
17:12 manual alignment of sample position; no laser alignment, but green crosses on monitor.
The flow cell cannot be driven in vertical direction with any motor, so no absorption can be carried out.
- filenumbers #55363, #55364, #55365

## empty flow cell and empty capillary for background
17:56: empty sample environment
- 5 s: 55368, #55366 - 55368 have x-axis from 0 to ~35 instead of 0 to ~3500
- 60 s / 10 frames: #55369
18:20: empty capillary
- 





