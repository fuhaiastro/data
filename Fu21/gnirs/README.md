## Observations
Gemini Program ID: GN-2017A-Q-31  
Observation date: 2017 Feb 19  
Cross-dispersed mode with the 32 l/mm grating

## How to read the data products in IDL

```idl
; load stacked 2D spec
stack = mrdfits('sci2d.fits',1,/silent) ; DN/s
; load wavelength calibration
wave = mrdfits('wavecal.fits',1,/silent)
; load combined 1d spec from boxcar extraction
spec = mrdfits('box1dct.fits',0,h) ; DN/s

; load telluric star spectra
; HIP49125     10 01 35.421 -01 01 05.23 2000.0 vmag=7.19 A0 hmag=6.634
std2d = mrdfits('std2d.fits',1,/silent) ; DN/s
std1d = mrdfits('std1dc.fits',0,h) ; DN/s
```
