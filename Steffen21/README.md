# Close Galaxy Pairs and Multiples in MaNGA IFUs

table1_mrt.txt is the machine readable table published in Steffen et al. (2021), "SDSS-IV MaNGA: The Radial Profile of Enhanced Star Formation in Close Galaxy Pairs"

This table lists a total of 404 plate-IFUs that contain close galaxy pairs and multiples in the eighth MaNGA Product Launch (MPL-8). The second column lists the component index, where ''0'' indicates the primary target of the MaNGA observation. For each IFU, all components within 2000 km/s of the primary are listed, sorted in ascending angular distance from the primary.

To load the table in IDL, use
```idl
data = read_fmr('table1_mrt.txt')                                
help,data.data
```
