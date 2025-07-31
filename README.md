# FIR Filter Design Using Windowing Techniques

This project focuses on the design and understanding of Finite Impulse Response (FIR) filters using various windowing methods. FIR filters are a key component in digital signal processing, known for their simplicity, inherent stability, and ability to maintain linear phase characteristics.

---

## 📚 Objective

The goal of this project is to demonstrate how FIR filters can be designed using window-based techniques and to analyze the impact of different window functions on the filter's behavior.

---

## 📘 What is an FIR Filter?

An FIR (Finite Impulse Response) filter is a type of digital filter where the output is determined by a finite number of past input samples and a fixed set of coefficients. Unlike IIR (Infinite Impulse Response) filters, FIR filters do not use feedback and are always stable.

---

## 🛠️ Design Approach

1. **Start with an ideal frequency response**  
   For example, in the case of a low-pass filter, the ideal response allows all frequencies below a cutoff frequency and blocks those above it.

2. **Compute the corresponding impulse response**  
   This ideal impulse response typically extends infinitely in both directions, which makes it impractical to implement directly.

3. **Truncate the impulse response**  
   Since real systems cannot handle infinite-length signals, the impulse response is cut off to a finite number of points.

4. **Apply a window function**  
   Truncating abruptly can introduce artifacts (like ripples in the frequency domain). A window function smooths the edges of the truncated signal, improving the filter's performance by reducing side lobes and controlling transition bandwidth.

---

## 🪟 Window Functions Used

- **Hamming Window**: Reduces side lobes moderately; commonly used.
- **Hanning Window**: Offers better transition smoothness but slightly wider main lobe.
- **Blackman Window**: Provides better attenuation of side lobes but with a wider transition band.

Each window affects the filter's frequency characteristics differently — there is always a trade-off between main lobe width (sharpness of transition) and side lobe attenuation (leakage control).

---

## 📊 Frequency Response

The frequency response of the FIR filter shows how different frequencies are attenuated or passed. A well-designed filter will have:
- A flat passband (where frequencies are preserved)
- A sharp transition band (between pass and stop bands)
- A suppressed stopband (where frequencies are attenuated)

---

## 🧰 Tools and Technologies

- **Programming Language**: Python  
- **Libraries Used**: NumPy, SciPy, Matplotlib  
- **Platform**: Jupyter Notebook

---


