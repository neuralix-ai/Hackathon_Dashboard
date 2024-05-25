# Hackathon: Interactive Dashboards to Showcase Jupyter Notebook Visualizations

## Objective
Identify talented undergraduate seniors for data visualization internships by testing their skills in creating interactive web UIs using data visualization libraries, with a focus on H2O Wave. Participants will be provided with a Jupyter notebook containing data processing and Plotly visualizations, as well as a mockup of the desired dashboard. Their task will be to quickly create a dashboard that displays the desired plots without backend overhead.

## Duration
One week

## Provided Resources
- A Jupyter notebook with data processing steps and Plotly visualizations.
- A .csv and .pkl file containing time series data.
- Mockup slides of the desired dashboard.
- API keys for using ChatGPT to assist development.

## Challenge Overview

### Stage 1: Static Elements

#### Preset File and Time Series Display
- Create separate, navigable pages with a hierarchical list of pages according to the dashboard mockup slides.
- Display charts relevant to each dashboard page.
- Display simple statistics (mean, median, etc.).
- Theme the dashboard to match our company’s website using screenshots for reference.

### Stage 2: Interactive Elements

#### Dynamic Navigation and Interaction
- Enable navigation by clicking on specific elements that act as links to other pages of the dashboard.
- Display valuable meta-data when hovering over information such as specific times and values.

### Stage 3: Auto-Generating Dashboards Using LLMs

#### LLM Integration
- Set up a large language model (e.g., ChatGPT) to assist data scientists in generating similar dashboards from Jupyter notebook code.

## Evaluation Criteria
- **Functionality:** We expect approximate solutions that are not exact replicas but give the impression of completion.
- **Usability:** Ensure functionality is provided only where desired.
- **Innovation:** Apply creative approaches to address challenges or issues with specific requests.
- **Technical Skills:** Show adaptability and proficiency in adopting new tools and libraries with the assistance of large language models (LLMs).
- **Adherence to Guidelines:** Following the provided theme and utilizing the resources effectively.

## Submission Guidelines
- Submit the complete interactive dashboard application.
- Provide a brief documentation explaining the design and functionality.
- Include any additional code or resources used in the development process.

## Prizes
- The winner will be offered an internship position at our company.
- All submissions will be reviewed for potential inclusion in our future projects, with due credit given to the creators.

## Motivation
In our fast-paced startup, the ability to quickly demonstrate the value of our data science models to potential clients is crucial. Imagine a scenario where our data science team has developed a powerful new algorithm for predicting equipment failure. They have all the data and initial visualizations in a Jupyter notebook, but transforming this into a polished, production-ready dashboard is a time-consuming process that requires significant collaboration with our software engineering team.

This lag can mean missed opportunities, as clients need to see the potential of our models immediately. We need someone who can bridge this gap, rapidly implementing visualizations that effectively showcase our data science work without the lengthy development cycle. This ability to create temporary, yet interactive and insightful dashboards directly from Jupyter notebooks will enable us to present our solutions dynamically, adapt quickly to client feedback, and secure new business opportunities.

## Details

### Sources
- **Code:** Github
- **Visualization:** H2O Wave
- **ChatGPT API Key:** please request from ryan@neuralix.ai

## Project Folder Structure
The project directory is organized as follows:
```
Dashboard
│
├── Dashboard References  
│ ├── PythonPlots  
│ │   └── Directory containing .png and .json examples of  
│ │       various Python-generated plots used in the dashboard.  
│ ├── Slides.pdf  
│ │   └── A mockup of how the dashboard structure.  
│ └── WebUI.png  
│     └── A screenshot of the web UI for the dashboard slides.  
│  
├── Data  
│ ├── Slide6-8.pkl  
│ │   └── Pickle file containing data for slides 6 & 8  
│ └── T1.csv  
│     └── CSV file with wind turbine data.  
│  
├── Notebooks  
│ ├── TimeSeriesVisualization.ipynb  
│ │   └── Jupyter notebook for visualizing time series data.  
│ └── TurbineLevelVisualization.ipynb  
│     └── Jupyter notebook for visualizing turbine data.  
│  
└── Output  
    └── Folder for storing output files generated by the notebooks  
        and data processing scripts.  
```

## Dashboard Structure
The intent of the dashboard is to show data at three levels:
1. The top level shows an operational summary of a wind farm.
2. The mid level gives an overview of specific failures or predicted failures.
3. The bottom level shows specific bearing failures or predicted failures.

There are a total of 8 dashboard pages we would like created. Clicking on some elements of the dashboard should link to other pages. These are indicated by the mouse pointers and slide numbers in Slides.pdf. We do not need full interactivity of the plots. For example, on slide 2, There can be a transparent clickable box over a red turbine which redirects to slide 3. The goal of this whole project is to gauge customer interest in the dashboard, rather than demonstrating full functionality of the dashboard. Please imply functionality wherever possible, though include functionality if it is straightforward.

## Visualizations
All of the visualizations have a python implementation in one of the two jupyter notebooks. If it is possible to directly use this code on a dashboard, that is ideal. If you must use one of the predefined H2O Wave plots, then use the python code as a reference.

Some of the visualizations in Slides.pdf may be non-standard. If you can synthesize a new plot, that’s great, but if not, try to visualize it another way. If it’s too complex, leave a placeholder and come back to it later.

We are most interested in an implementation that will take as few steps as possible to transition from a python plotly visualization to a dashboard. We are suggesting H2O Wave because it has been straightforward in our experience, but if you are familiar with another method, go for it. Remember, the goal is rapid prototyping.

### Priorities in Dashboard References
- **WebUI.png** demonstrates how the web page should look
- **Slides.pdf** demonstrates how each visualization should look.
- **PythonPlots** are the output of jupyter notebooks, which demonstrate how the plots may be implemented.

## Note
Participants are encouraged to use ChatGPT and other available resources to assist in their development process. We do not expect all stages to be completed fully but aim to see how participants approach the problem and their potential to contribute to our team.