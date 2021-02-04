## Observations
ESO Program: 089.A-0855  
Dates: 2013 March 31 and 2013 May 1  
Telescope: VLT/UT2

## How to read the FITS files in IDL

```IDL
infile = 'J0913-0107_bg_XSHOOTER.fits' ; QSO1 at z = 2.92
infile = 'J0913-0107_fg_XSHOOTER.fits' ; QSO2 at z = 2.75
; load spectrum and continuum fit
flux = mrdfits(infile,0,/silent)
ferr = mrdfits(infile,1,/silent)
wave = mrdfits(infile,2,/silent)
cont = mrdfits(infile,3,/silent)
; normalize spectrum by continuum fit
nflux = flux/cont
nferr = ferr/cont
```
