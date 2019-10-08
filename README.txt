 1 This repository stores an Arduino program to sample data for ISFET testing. Data is transmitted to a Raspberry Pi or ser    ial monitor using serial communication. The program accepts user input to set sampling rate and form of data to transmit    , as ADC output, millivolt results, or both. Data is transmitted in .csv format.
  2 
  3 Data is reported in the following format for ADC or millivolt results:
  4 
  5         vsd,vplus,vout,isd,temp,gnd
  6         
  7 Data is reported in the following format when the "both" option is selected:
  8 
  9         vsd_adc,vplus_adc,vout_adc,isd_adc,temp_adc,gnd_adc,vsd_mv,vplus_mv,vout_mv,_isd_mv,temp_mv,gnd_mv
 10         
 11 When connected to a Raspberry Pi, the Pi python script appends a time stamp in milliseconds:
 12 
 13         timestamp,vsd,vplus,vout,isd,temp,gnd 

