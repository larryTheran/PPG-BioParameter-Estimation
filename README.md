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

![Detrended_625_test](https://user-images.githubusercontent.com/55849820/153887477-7a4b3469-ec63-447f-b27d-d2561da8cbf8.png)


# Thresholding to Find Peaks of Interest


![peack_4wave](https://user-images.githubusercontent.com/55849820/153887578-18e65ba8-628d-413a-b04c-491397a6e129.png)


# Spectral Response
The data for the extinction coefficient:

![SharedScreenshot4](https://user-images.githubusercontent.com/55849820/153889671-dc760b93-31d4-43eb-9b13-a7e908b5dd9f.jpg)

# Ratio of the molar extinction coefficients for Hb and HbO2


![SharedScreenshot5](https://user-images.githubusercontent.com/55849820/153916144-8c45f658-ba2a-4e3f-90b3-aecdd07db6ce.jpg)


# Oxigen Saturation
If we use we use only functional Hemoglobin and two wavelengths as in the case of the pulse oximeter, then the absorption will be:

![SharedScreenshot](https://user-images.githubusercontent.com/55849820/153888381-87a74f87-eb68-43d7-9dba-ab34fdb0bf6e.jpg)

The ratio of the absorbance at two wavelengths:

![SharedScreenshot2](https://user-images.githubusercontent.com/55849820/153888551-f003dc04-d504-4ab5-aef4-2bbdff0e7ed8.jpg)

Assuming that the optical path length of the two-wavelength is equal to 'd' can be removed in the ratio. W can rewrite the equation as a function of the ratio to calculate de Oxygen saturation.

![SharedScreenshot3](https://user-images.githubusercontent.com/55849820/153888820-d7bfb31d-2a28-409e-9672-a1ae545dee7d.jpg)

# Hemoglobin measurements
In the case of the hemoglobin concentration prediction, in the last section, we got that the absorption for a different substance was given by: 


![Spectra4Hemo](https://user-images.githubusercontent.com/55849820/153916583-8e7c4e93-96ed-4ca9-a2cc-a58e7e4972a8.jpg)








