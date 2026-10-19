# AppStar — Interactive Stellar Evolution & Hertzsprung–Russell Diagram

**UTS 36104 Data Visualisation and Narratives — Session 2 Part D (Stars)**

An interactive web application exploring stellar astrophysics, stellar evolution, and the Hertzsprung–Russell (H–R) diagram across mass, age, and metallicity.

## Features
- **Metallicity Slider:** Interactive Streamlit slider controlling $\log_{10} Z$ from $-4.0$ to $-1.4$. Rebuilding the grid on release adjusts lifetimes ($Z^{0.1}$), brightness, and remnant boundaries.
- **Pair-Instability Supernova Branch:** Implements the $140 \le M \le 260\,M_\odot$ zero-metallicity ($Z < 0.001$) disruption branch where stars blow apart leaving no remnant.
- **Interactive H–R Diagram in Altair:**
  - Logarithmic reversed surface temperature axis ($45,000\,\text{K}$ down to $2,200\,\text{K}$).
  - Logarithmic luminosity axis ($10^{-4}$ to $10^6\,L_\odot$).
  - Static Main Sequence reference track derived from $L = M^{3.5}$ and $T = T_\odot M^{0.475}$.
  - Real-time animated star riding mass and age sliders.

## Running Locally
```bash
pip install -r requirements.txt
streamlit run star_app.py
```
