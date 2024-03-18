# Dataset link
https://www.kaggle.com/datasets/iamsouravbanerjee/world-population-dataset

# World-Population-Data-Analysis
This project looks at how populations in different countries and territories have changed over time, giving us ideas about growth, patterns, and where they stand compared to each other.

# Key Findings
The world's population has grown a lot, reaching over 7.5 billion in 2019. China and India are the biggest, each with over 1 billion people. India is expected to become the most populous by 2030, passing China. This data covers the 11 most populated countries, all with over 100 million people. Population growth has slowed since the 1970s, but it's still expected to reach over 10 billion by 2055.

plt.figure(figsize=(15, 6))
labels = columns_reversed #{columns_reversed = columns[::-1]} using this code for reversing the column's names
world_population_filtered = [world_population[columns.index(year)] for year in columns_reversed]
plt.plot(labels, world_population_filtered, marker='o', linestyle='-')
plt.xlabel('Years')
plt.ylabel('Population')
plt.grid()
plt.title('World Population Over the Years')
plt.show()
