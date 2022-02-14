# PPG-BioParameter-Estimation
Improvement of the accuracy of wearable optical devices may be achieved by a model that integrate a characterization of optical signals with the skin properties and its combination with Deep Learning methods. This Repo focuses on using the data from a Noninvasive Light-Based Platform for Signal Processing required to get correct PPG signal from a base photometric device.

The normal range for hemoglobin is:
For man: 13.5 to 17.5 grams per deciliter (g/dL)——————8.7 to 11.2 Molly/L (SI units)
For women: 12.0 to 15.5 grams per deciliter


# PPG Real DATA

![PPG_variation_5Wave_60s](https://user-images.githubusercontent.com/55849820/153887105-a8a42eb0-bd09-4f8c-9533-460c56e109b9.png)


# Detrending Data
The above signal shows a baseline shift and therefore does not represent the true amplitude. In order to remove the trend, fit a low order polynomial to the signal and use the polynomial to detrend it.


![PPG_variation_5Wave_60s_BaselineShift](https://user-images.githubusercontent.com/55849820/153887180-dc3f80ce-7a47-478d-a050-8245901ed80f.png)
