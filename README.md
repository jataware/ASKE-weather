### ASKE COUNTY-LEVEL Weather Data

### Background

The major parameters in this file are sequential climatic county  monthly 
maximum, minimum and average temperature (deg. F. to 10ths) and precipitation (inches to 100ths). 
Period of record is 1895 through latest month available, updated 
monthly.

Values from the most recent two calendar years will be updated on a monthly 
basis.  Period of record updates will occur when the underlying data set 
undergoes a version change.

METHODOLOGY:

County values in nClimDiv were derived from area-weighted averages of 
grid-point estimates interpolated from station data.  A nominal grid resolution
of 5 km was used to ensure that all divisions had sufficient spatial sampling 
(only four small divisions had less than 100 points) and because the impact of 
elevation on precipitation is minimal below 5 km.  Station data were gridded 
via climatologically aided interpolation to minimize biases from topographic 
and network variability.

The Global Historical Climatology Network (GHCN)  Daily dataset is the source 
of station data for nClimDiv.  GHCN-Daily contains several major observing 
networks in North America, five of which are used here.  The primary network 
is the National Weather Service (NWS) Cooperative Observing (COOP) program, 
which consists of stations operated by volunteers as well as by agencies such 
as the Federal Aviation Administration.

Data is updated monthly.

### Code Overview
1. #### Auto Download county weather data from NOAA at: ftp://ftp.ncdc.noaa.gov/pub/data/cirs/climdiv/
  - Data: precipitation (inches), Tmax (<sup>o</sup>F), Tmin(<sup>o</sup>F), Tavg(<sup>o</sup>F)

  - These county-level files are downloaded to your working directory
  
    - climdiv-pcpncy-vx.y.z-YYYYMMDD

    - climdiv-tmaxcy-vx.y.z-YYYYMMDD

    - climdiv-tmincy-vx.y.z-YYYYMMDD
    
    - climdiv-tmpccy-vx.y.z-YYYYMMDD  
      

2. ####  Read in FIPS transforms: NOAA uses different state FIPS codes 
  
  - You will need these files in the /noaa_to_census directory for required FIPS transforms

    - `noaa_fips.txt`

    - `noaa_states.txt`

    - `state_fips.txt`
    
3. ####  Read in NOAA data (dataframes)

4. ####  Format dataframes (year filter and pivot to usable form)

5. ####  Write formatted data file to working directory
