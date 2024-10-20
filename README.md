# assignment_github
Harmonic analysis of AC signals
<br>
It involves breaking down of complex,non sinusoidal waveform into its fundamental frequency and various harmonic components.

# Step 1 - Fourier Transform
Implementation of Fourier analysis for extracting harmonic components from AC signals using Python. This example will simulate an AC signal composed of a fundamental frequency (50 Hz) and its harmonics (150 Hz and 250 Hz) and we will apply the Fast Fourier Transform (FFT) to extract these components.
We'll use Python libraries like numpy for signal processing and matplotlib for visualization.

Steps in the Implementation:
Generate a synthetic AC signal with a known fundamental frequency and harmonics.
Apply FFT to extract frequency components.
Display the results to identify harmonic frequencies.

# Step 2 - THD Computation and results in form of plots
THD is a measure of the harmonic distortion present in a signal and is typically calculated as the ratio of the sum of the powers of all harmonics to the power of the fundamental frequency.

Steps in the Implementation:
Perform FFT to extract the fundamental and harmonic frequencies.
Calculate the THD based on the ratio of harmonic amplitudes to the fundamental.
Plot the frequency spectrum and display the calculated THD value.

# Step 3 - Providing sample signals for testing
Generates multiple sample signals: These signals have different harmonic contents, simulating different levels of distortion.
Performs FFT and calculates the THD for each signal.
Plots the time-domain signal, the frequency spectrum, and shows the THD for each case.

Test Signals:
The test_signals list contains different test cases:
Test 1: A pure sine wave (no harmonics, THD should be 0%).
Test 2: A signal with a 50 Hz fundamental and a 3rd harmonic (150 Hz).
Test 3: A signal with 50 Hz fundamental, 3rd harmonic (150 Hz), and 5th harmonic (250 Hz).
Test 4: A signal with 50 Hz fundamental, 3rd, 5th, and 7th harmonics (150 Hz, 250 Hz, and 350 Hz).

Plotting:
For each test signal, the code plots both the time-domain waveform and the frequency spectrum. The THD value is displayed in the plot title and printed to the console.
