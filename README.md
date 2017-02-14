# StepCounter
StepCount: An Android App that that samples accelerometer to count steps, using the peak detection

The Accelerometer data is gathered and processed in real-time. The implementation is intended to be device agnostic, with
self-adjusting parameters, tuning to the sampling rate of the sensor in your device. 

This has been tested on a Google Pixel XL (Sampling rate = ~50HZ for SENSOR_DELAY_NORMAL)
The the data is sent through a low-pass filter with alpha = 0.1, timeconstand = 0.18

Also includes a simple time-based jitter filtration method to eliminate unrealistic step counts 