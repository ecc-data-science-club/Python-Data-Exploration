
# Visualizing the data with matplotlib 

## Plots

### Bar plot
X = np.arange(10)
Y = np.random.uniform(0, 1, 100)
ax.bar(X, Y)

### Box plot
Z = np.random.normal(0, 1, (100, 3))
ax.boxplot(Z)

### Scatter plot
X = np.random.uniform(0, 1, 100)
Y = np.random.uniform(0, 1, 100)
ax.scatter(X, Y)

### Pie chart
Z = np.random.uniform(0, 1, 4)
ax.pie(Z)

### Histogram
Z = np.random.normal(0, 1, 100)
ax.hist(Z)

### Print Plot
plt.show()


## Modifying plots 

### Color
X = np.linspace(0, 10, 100)
Y = np.sin(X)
ax.plot(X, Y, color=”black”)

### Range of colors (one method for a histogram, there are many options)
X = np.random.randn(1000, 4)
cmap = plt.get_cmap(“Oranges”)
colors = cmap([0.2, 0.4, 0.6, 0.8])
ax.hist(X, 2, histtype=’bar’, color=colors)

### Line style (to dashed)
X = np.linspace(0, 10, 100)
Y = np.sin(X)
ax.plot(X, Y, linestyle=”--”)

### Line thickness
X = np.linspace(0, 10, 100)
Y = np.sin(X)
ax.plot(X, Y, linewidth=5)

### Adding ticks
X = np.linspace(0, 10, 100)
Y = np.sin(X)
ax.plot(X, Y, marker=”0”)

### Setting Labels
ax.plot(X, Y)
ax.set_ylabel(None)
ax.set_xlabel(“Time”)





