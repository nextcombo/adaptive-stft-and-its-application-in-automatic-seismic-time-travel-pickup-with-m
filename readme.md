# Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]

Keywords: Short-time Fourier Transform, Instantaneous window length, Instantaneous travel time, Seismic coherency picking.
Introduction: Time-frequency analysis has been thriving in various research and applications in recent years due to the fact that most signals encountered in practice are not stationary. Time-frequency analysis can simultaneously analyze signals in both the time domain and spectral domain, thus revealing comprehensive information about non-stationary signals. Some popular conventional time-frequency representations (TFR) include Short-Time Fourier Transform (STFT), Wigner-Ville distribution (WVD), Wavelet transform (WT), and S transform (Pei et al., 2012). In ideal conditions, TFR should only reveal the spectral information of the signal occurring at any given moment. Therefore, the main purpose of TFR is to provide a more concentrated TF energy distribution without cross terms, allowing it to be as close to an ideal TFR as possible. Thus, we attempt to achieve this by finding an adaptive instantaneous window length. Additionally, coherency picking is an important step in seismic processing. It is used for static correction, velocity analysis, seismic tomography, amplitude-offset analysis, and geological interpretation. This new arrival of seismic energy is represented by discontinuities in values of one or more attributes characterizing different layers underground (Saragiotis et al., 2013). Here we refer to a set of arrangements on several traces of an earthquake record, which indicates the arrival of new seismic energy. For this purpose, we utilize adaptive STFT analysis.
Main principles
MATLAB part of the program clc, clear\nload SignalsTypes.mat Signals\ns = Signals.S.HypChirps'; \ndt = Signals.S.dt; \nN = length(s); \n​\n[ G, ~, ~, W, H ] = AdaptiveSTFT( s, 'simple'); \nfigure\nimagesc(H)\nfigure\nimagesc(W)\nfigure\nimagesc(G) \n​\nfigure\n[ G, CF ] = AdaptiveSTFT( s, 'adaptive', 'pow2', 1 ); \nimagesc(G)\nfigure\nplot(CF)\nfigure\n[ G, ~, P, W ] = AdaptiveSTFT( s, 'adaptive', 'pow2', 2 ); \nimagesc(W)\nfigure\nimagesc(G)\nfigure\nplot(P)\nMATLAB Simulation Results
End

## Images

![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](01.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](02.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](03.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](04.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](05.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](06.jpg)
![Adaptive STFT and its application in automatic seismic time-travel pickup [with MATLAB code]](07.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
