## Observations
Gemini Program ID: GN-2017A-Q-31  
Observation date: 2017 Feb 19  
Cross-dispersed mode with the 32 l/mm grating

## How to read the data products in IDL

```idl
; load stacked 2D spec
stack = mrdfits('sci2d.fits',1,/silent)
; load wavelength calibration
wave = mrdfits('wavecal.fits',1,/silent)
; load calibrated 1d spec
spec = mrdfits('sci1dct.fits',0,h) ; erg/s/cm2/A
```
