# Checklist

## ToDo:
- [x] optimize flow cell T pice thermocouple connection, too flimsy/complex now
- [ ] Get used to linux
  - Script/mask creation with: pyFAI-calib2 
- [x] ceck 1_tobuy.md 
- [ ] Workflow for dpf/dxrd pdfgetx3
- [x] learn pyFAI-integrate
- [x] learn xpdtools
- [ ] Create easy to use image_to_iq script (for xpdtools)
- [ ] learn about the new detector
- [x] sample list
---

## Software
- better way to control MFCs, T controller simulataneously
- How to record MFC's 
- How to use the MS
---

## Detector
> _Arc_ Detector
Diamond
has developed the _ARC_ detector as the ideal detector for I 15 1
Photon counting capabilities and high detection efficiency make it the perfect tool for accurately measuring weak diffuse scattering data at high Q. The 4.7 megapixel detector consists of 24 modules arranged on an arc at a radius of 250 mm, giving an angular 2θ coverage of 83°. The _ARC_ will be
able to run in different modes, depending on the time reciprocal and real
space resolution requirements of the experiment In rapid mode, the ARC will
be able to collect data to a $Q_{max}$ of 27 $Å^{-1}$ (at 76 keV) at a rate of up to 50 Hz. Longer collections at two 2θ positions will give sample limited PDF data with $Q_{max}$ 51 $Å^{-1}$ (at 76 keV), or $Q_{max}$ 27 $Å^{-1}$ at 40 keV if higher resolution reciprocal space data is also needed.

<div style="text-align:center">
    <img src="./images/arcdetector.png" alt="Figure of the new arc detector" style =width:75%>
    <p><em>Figure a: a) Engineering drawing of the ARC on its goniometer, b) internals of the ARC during assembly and c) the completed ARC during testing on I 15 1</em></p>
</div>

- maximum counts per pixel (count rate)
- what about the gaps between the modules (does it result in some sort of kinks during the integration?)
- what reset intervals to chose (should not interfer with experimental timings)
- how long do the experiments take
- does the detector need to be reset in between sets?
- ...
---

## Remeasure 
- What $ex-situ$ sample need to be remeasured from DESY P02.1
