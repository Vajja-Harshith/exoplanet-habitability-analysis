# NASA Exoplanet Habitability Analysis

This is a self-directed data science project I built to sort through the noise of the NASA Exoplanet Archive. I wanted to see if I could use basic Python tools to replicate how astrobiologists score planet habitability.

### The Goal
Out of nearly 40,000 planet observations, how many are actually similar to Earth? (Spoiler: Not many. Most are scorching hot gas giants that orbit their stars in less than 20 days).

### What I Did:
1. **Data Cleaning:** Loaded the raw NASA dataset using Pandas and threw out columns/rows with missing radius (`pl_rade`) or temperature (`pl_eqt`) data.
2. **The Algorithm:** Coded a simplified Earth Similarity Index (ESI) using a weighted geometric mean. I matched each planet's radius against Earth (1.0) and its equilibrium temperature against Earth's baseline (255 Kelvin).
3. **Visualization:** Used Matplotlib and Seaborn to plot the massive cloud of discovered planets, highlighting the 9 actual "Goldilocks Zone" candidates in bright green. 

### What I Learned:
I started this project with zero Python knowledge. Building this taught me how to read documentation, handle massive CSV files without crashing my browser, and use NumPy for basic geometric formulas. Most importantly, it proved to me that data tells better stories than textbooks.

Top candidate found: **Kepler-452 b** (ESI: 0.93)
