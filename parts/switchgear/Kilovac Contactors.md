# Kilovac Contactors

Can be a bit awkward to mount, as the flange-on-a-can design can make access to mounting bolts a bit tricky - strongly suggest using a long insulated screwdriver and screw bolts rather than hex-head for this.

No internal economiser on any models readily available by the usual channels either, so using some kind of external econimising circuit is _strongly_ advised, as otherwise most BMS/Controllers will quite happily drive the coils at whatever voltage your pack puts out, so even getting a 48v rated coil one on my 48v system results in a drive voltage of around 60v when the cells are fully charged, and the coils then get very hot.

Suggested circuitry for this is a passive resitor and capacitor in parallel with one another, connected to in series to the coil line.
Tune your resistor to be within the holding current range for your contactor (measure the internal resistance of your coil and min/max battery voltages to calculate this) then select a capacitor which has a high enough voltage rating and around 100mF or thereabouts to have a solid peak to engage the armature that then backs off to the hold current over time.
Note that this is _not applicable_ for contactors or solenoids which have high switch frequencies, as they will end up being sat in the high-drive part of the curve constantly, and will never disengage.

Diagram TBD
