# Autoviz


AutoViz is an open-source Python library designed to simplify Exploratory Data Analysis (EDA) through automated, high-quality visualizations. With just a single line of code, AutoViz helps users detect patterns, spot trends, and assess data quality effortlessly. Whether you're a beginner in data analysis or a seasoned data scientist.

AutoViz 📊🚀
Automated Exploratory Data Analysis (EDA) with One Line of Code!

🔹 What is AutoViz?
AutoViz is an open-source Python library designed to simplify Exploratory Data Analysis (EDA) through automated, high-quality visualizations. With just a single line of code, AutoViz helps users detect patterns, spot trends, and assess data quality effortlessly. Whether you're a beginner in data analysis or a seasoned data scientist, AutoViz speeds up your workflow and enhances insights.

✨ Key Features
✅ Ease of Use – No complex coding, just plug and play
✅ Speed – Instantly generate multiple visualizations
✅ Scalability – Handles datasets of all sizes efficiently
✅ Automation – AutoViz selects the best visualization types
✅ Customization – Modify chart types, color palettes, and more
✅ Data Quality Insights – Built-in FixDQ() function for quick data quality fixes

⚡ Installation
Install AutoViz via pip:



pip install autoviz
For specific Python versions:


pip install -r requirements.txt   # For Python <3.10
pip install -r requirements-py310.txt  # For Python 3.10
pip install -r requirements-py311.txt  # For Python 3.11+
📌 How to Use
Quickly visualize a dataset with just one line of code:


from autoviz import AutoViz_Class

AV = AutoViz_Class()
dft = AV.AutoViz("your_file.csv")
🔗 See More Examples

📊 Visualization Output
AutoViz supports multiple visualization formats:
📌 Static charts (png, svg, jpg)
📌 Interactive charts (bokeh, html)
📌 Dashboards for exploratory analysis (server mode)

💡 Why Choose AutoViz?
Unlike other EDA tools, AutoViz:

Automates the selection of best-fit visualizations
Supports large datasets without performance lag
Integrates seamlessly with Pandas and Jupyter Notebooks
Offers built-in data quality assessment and fixes

🤝 Contributing
AutoViz is an open-source project, and we welcome contributions! 🚀
🔹 Submit bug reports or feature requests in Issues
🔹 Help improve the code – see CONTRIBUTING.md
🔹 Spread the word by ⭐ starring the repository!


📌 AutoViz is here to make EDA faster, smarter, and easier. Try it today! 🚀🔍


AutoViz 📊🚀 – The One-Line Automatic Data Visualization Library
(Optional: Replace with your actual logo image link)

Unlock the power of AutoViz to visualize any dataset—any size—with just a single line of code!
Now with data quality assessment and automatic fixes via the FixDQ() function.


🎯 Why AutoViz?
AutoViz is an AI-powered exploratory data analysis (EDA) tool that automatically visualizes datasets in seconds. Whether you're a beginner or an expert, AutoViz simplifies data exploration and pattern detection.

🔹 Automated Insights – Generates insightful charts effortlessly
🔹 Works with Any Dataset – Handles small to massive datasets
🔹 Interactive & Static Visuals – Supports Matplotlib, Bokeh, Dashboards, and HTML Exports
🔹 Fix Data Quality Issues – AutoViz now detects and fixes data quality (DQ) problems in a single command!
🔹 Seamless Integration – Works with Jupyter Notebooks, Pandas, CSVs, JSON, and More

🚀 Installation
AutoViz is available via PyPI and can be installed in seconds:


pip install autoviz
For different Python versions:


pip install -r requirements.txt   # Python <3.10  
pip install -r requirements-py310.txt  # Python 3.10  
pip install -r requirements-py311.txt  # Python 3.11+  
🛠 Prerequisites:

Python 3.7+
Anaconda (Optional but recommended for an isolated environment)
For developers & contributors:


git clone https://github.com/AutoViML/AutoViz.git
cd AutoViz
pip install -r requirements.txt
📌 How to Use AutoViz
🔹 Generate Instant Visualizations with just one line of code:


from autoviz import AutoViz_Class

AV = AutoViz_Class()
dft = AV.AutoViz("your_file.csv")  # Provide a CSV, JSON, or Pandas dataframe
🔹 Use AutoViz with a Pandas DataFrame:


import pandas as pd
from autoviz import AutoViz_Class

df = pd.read_csv("your_data.csv")
AV = AutoViz_Class()
dft = AV.AutoViz("", dfte=df)
🔹 Fix Data Quality Issues Automatically:


from autoviz import FixDQ

clean_df = FixDQ(df)
🔹 Customize Visualizations:


dft = AV.AutoViz(filename, chart_format="bokeh", verbose=2)
📌 View More Examples

📊 What Does AutoViz Generate?
AutoViz automatically selects the best visualizations for: ✔ Data distributions
✔ Correlation matrices
✔ Time series trends
✔ Categorical vs. numerical insights
✔ Outlier detection
✔ Feature importance graphs

💡 Interactive Mode: Use chart_format="bokeh" to generate interactive charts for deeper analysis!

🛠 API and Configurations
You can customize AutoViz using various parameters:


AV.AutoViz(
    filename="your_file.csv",  # Path to file (CSV, JSON, etc.)
    sep=",",                   # Separator (default: comma)
    depVar="target_column",     # Target variable (optional)
    dfte=None,                  # Pandas DataFrame (if no filename)
    verbose=1,                  # Display level (0 = minimal, 1 = standard, 2 = save plots)
    chart_format="bokeh",       # Available: "png", "svg", "jpg", "bokeh", "server", "html"
    max_rows_analyzed=150000,   # Sample large datasets
    max_cols_analyzed=30        # Limit number of visualized columns
)
📌 Full API Reference

📈 Examples
Here are some quick-use cases:

Example 1: Visualizing a CSV File

AV = AutoViz_Class()
dft = AV.AutoViz("data.csv")
Example 2: Using a Pandas DataFrame

import pandas as pd
df = pd.read_csv("data.csv")
AV = AutoViz_Class()
dft = AV.AutoViz("", dfte=df)
Example 3: Generating Interactive Charts

dft = AV.AutoViz("data.csv", chart_format="bokeh")
Example 4: Saving Plots

dft = AV.AutoViz("data.csv", verbose=2, save_plot_dir="visuals/")
📌 Explore More Examples

👥 Contributors & Maintainers
AutoViz is actively maintained by the AutoViML team and contributors.
Want to contribute? Follow our Contribution Guidelines 🚀

Core Contributors:
🔹 @AutoViML, AnwarHussain-1011
🔹 @morenoh149
🔹 @hironroy

🙌 Special Thanks to our community contributors!

📜 License
AutoViz is released under the Apache License 2.0.
📌 Read the Full License

🤝 Contributing
Want to improve AutoViz? Join us!
🔹 Fork the Repo
🔹 Make Your Changes
🔹 Submit a Pull Request

📌 Read the Contribution Guide

📢 Stay Updated
📌 Changelog & Updates
📌 GitHub Issues
📌 Google Scholar Citations

🔹 Join the Discussion! – GitHub Discussions
🔹 Follow Us for More Updates!

Your feedback matters! If you have any issues or feature requests, submit a GitHub issue or join our community discussions.

🚀 AutoViz is ready to launch! Start visualizing your data effortlessly! 🎉
⭐ Star the repository & spread the word! 💡

📌 Visit AutoViz on GitHub
