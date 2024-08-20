
# 🏷️ NOTE:
- The answer notebooks (`labsheet_01_task01.py`, `labsheet_01_task02.py`) are available in the repository.


# Deep Learning – Lab 1
### Objective

This lab aims to equip students with knowledge and skills related to Python libraries and frameworks commonly used in deep learning.

---

### Libraries Covered

- **Numpy:** A library for the Python programming language that supports large, multi-dimensional arrays and matrices, along with mathematical functions to operate on these arrays.

- **Matplotlib:** A library for creating static, animated, and interactive visualizations in Python.

- **Pandas:** A library written for Python for data manipulation and analysis.

- **Seaborn:** A Python data visualization library based on Matplotlib that provides a high-level interface.

---

### Resources

- **Lab Codes Repository:** [SE4050-DL-Lecture02](https://github.com/jeewaka-p/SE4050-DL-Lecture02)
- **Online Store Customer Dataset:** [Download from Kaggle](https://www.kaggle.com/datasets/mountboy/online-store-customer-data?resource=download)
- **Au Nano Particle Dataset:** [Download from Google Drive](https://drive.google.com/drive/folders/1_6-GpmILQB4-8rMf5oW604pP1Nx54dYx?usp=sharing)

---

### 🚀 Tasks

### 🏷️ Task 1

1. **Create a 4x4 Array from Exponential Distribution:**
   - Generate a random 4x4 array using Numpy from an exponential distribution.

2. **Visualize Distribution Histogram:**
   - Create a random 100000x1 array from the exponential distribution.
   - Visualize the histogram along with uniform and normal distributions. Modify the number of bins and plot view for better visualization.

   ```python
   plt.hist(np.random.rand(100000), density=True, bins=100, histtype="step", color="blue", label="rand")
   plt.axis([-2.5, 2.5, 0, 1.1])
   plt.legend(loc="upper left")
   plt.title("Random distributions")
   plt.xlabel("Value")
   plt.ylabel("Density")
   plt.show()

3. **3D Plot of \( Z = X^2 + Y^2 \):**
   - Using Matplotlib, plot \( Z = X^2 + Y^2 \) in a 3D plot. Limit the x and y values to [-5, 5].

4. **Correlation and Heatmap:**
   - Calculate the Pearson standard coefficient and Spearman rank correlation for the features [HP, Attack, Defense, Sp. Ark, Sp. Def, Speed] in the `seaborn_tutorial.ipynb`.
   - Visualize the results using heatmaps and ensure the values are displayed in the heatmap.

### 🏷️ Task 2: Working with the Au Nano Particle Dataset

1. **Filter and Create a New DataFrame:**
   - Download the `Au_nanoParticle_dataset.csv` and load the data into a new Colab notebook.
   - Filter the columns to exclude `N_total`, `N_bulk`, `N_surface`, and `R_avg` and create a new DataFrame.

2. **Display Data Samples:**
   - Display the first 20 samples of the new DataFrame.

3. **Statistical Analysis:**
   - Calculate the mean, standard deviation, and quartile values for each of the 4 features (`N_total`, `N_bulk`, `N_surface`, `R_avg`).

4. **Histogram Plotting:**
   - Plot the histogram of each of these features in a 1x4 layout.

5. **Pairplot Visualization:**
   - Visualize the scatter plots and histograms of the DataFrame using the `pairplot` functionality of the Seaborn library.

6. **Custom PairGrid Plot:**
   - Modify the following code to ensure that:
     - The diagonal plots contain the histogram of each feature along with the kernel density estimation plot.
     - The lower half [g.map_lower] contains the bivariate kernel density estimation plot.

      `#new_df` is the dataframe containing only the above mentioned 4 features.

   ```python
   g = sns.PairGrid(new_df)
   g.map_upper(sns.histplot)  # Bivariate histogram
   g.map_diag(sns.histplot)   # Histogram with KDE on diagonal
   g.map_lower(sns.kdeplot)   # Bivariate KDE plot

___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>


