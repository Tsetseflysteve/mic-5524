/*
 * This is a basic setup using the DHT11, I just needed to get it started, I recommend at least using a DHT22 or BME280 sensor.
 * The DHT11 is =/- 2 degrees and +/- 5% rH in its output. 
 * install the correct libraries and header files, although this is not pulling data directly from the internal algorithm you still need
 * to pre-heat and wake the sensor up.
 *
 *
 */

  /**
   * Gas type:
   * MICS-4514 You can get all gas concentration
   * MICS-5524 You can get the concentration of CH4, C2H5OH, H2, NH3, CO
   * MICS-2714 You can get the concentration of NO2
   *   CO       = 0x01  (Carbon Monoxide)  (1    - 1000)PPM
   *   CH4      = 0x02  (Methane)          (1000 - 25000)PPM
   *   C2H5OH   = 0x03  (Ethanol)          (10   - 500)PPM
   *   H2       = 0x06  (Hydrogen)         (1    - 1000)PPM
   *   NH3      = 0x08  (Ammonia)          (1    - 500)PPM
   *   NO2      = 0x0A  (Nitrogen Dioxide) (0.1  - 10)PPM
   *   
   *  
   *  Below is the data set from the Curve.
   *
   *  Gas           Rs    ppm    R0      ppm
   *
   *  H2S           0.7   0.1   0.6        0.5
   *  CO            0.0   0.1   0.01    1000 
   *  Ethanol       1.1   1.1   0.07     100 
   *  Hydrogen      0.8   1.05  0.04     200
   *  Ammonia       1.0   1.0   0.04     250
   *   Methane      0.75  1300  0.5    10100  
   *  Propane       0.17  1300  0.065  10100  
   *  Iso-butane    0.075 1300  0.06   10100
   */
