# Data Visualization

## Assignment 3: Final Project

### Requirements:
- We will finish this class by giving you the chance to use what you have learned in a practical context, by creating data visualizations from raw data. 
- Choose a dataset of interest from the [City of Toronto’s Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/) or [Ontario’s Open Data Catalogue](https://data.ontario.ca/). 
- Using Python and one other data visualization software (Excel or free alternative, Tableau Public, any other tool you prefer), create two distinct visualizations from your dataset of choice.  
- For each visualization, describe and justify:

    > DESCRIPTIONS & BACKGROUND
        - Dataset:
            - Outbreak data on healthcare providers of Toronto from Jan-Dec, 2024
            - File Name: ob_report_2024 (placed on my local repo). A snip of dataset shown in Appendix 2
            - URL: https://open.toronto.ca/dataset/outbreaks-in-toronto-healthcare-institutions/
            - Source of dataset: Toronto Public Health
            - Contact: edau@toronto.ca

        - Data Visualizations:
            - Python Code        Appendix 1
            - Box Plot:          "1. Python - Box PLot"
            - Stacked Bar Chart: "2. Python - Stacked Bar Chart"
            - Line Plot:         "3. Excel - Line Chart"
            - Bar Chart:         "4. Excel - Bar Chart"



    > What software did you use to create your data visualization?

        - Python for Box Plot & Stacked Bar Chart
        - Excel for the Line Chart & Bar Chart 


    > Who is your intended audience? 
      
        -Infection Prevention and Control practitioners
        -Public Health Officials 
        -Government Policy Makers
        -Healthcare Providers (Hospitals, Clinics, Doctors)
        -Epidemiologists
    
    > What information or message are you trying to convey with your visualization?

        -The Outbreak Dataset has the following info: Address & Name of Institution, Type of Facilities (Outbreak Setting), Type of Outbreak (respiratory, enteric, or other), Causative Agents, Date Outbreak Began, Date Declared Over, Active? (Y/N) 

        -The main goal of Outbreak Data Visualizatin is to convey critical insights that: 
            - Inform about the spread and severity of the outbreak.
            - Support decision-making for public health measures & resources allocation.
            - Raise awareness about trends, risks, and interventions.
            - Track interventions such as vaccination campaigns or social distancing policies.
        
        -My visualizations are just a few of many ways to inform the intended audiences or stakeholders re. the above goal without having to delve into the dataset itself as it has >1,000 records. 
            - Boxplot: tracking the Duration of Outbreak by Type of Facilities (Outbreak Setting). 
            - Stacked Bar Chart: tracking the No. of Outbreaks by Type of Facilities & the Causative Agent
            - Line Chart: Number of Outbreaks by Month in 2024
            - Bar Chart: Number of Outbreaks by Outbreak Types (respiratory, enteric, & others)
         
    
    > What design principles (substantive, perceptual, aesthetic) did you consider when making your visualization? How did you apply these principles? With what elements of your plots?

        -Because the stakeholders are highly educated in the field of Pulic Health with operational, strategic, & financial responsibilities, the emphasis has to be substance, facts, accuracy, & clarity, .
            - Primarily, I focused on Substantive Design i.e. content, accuracy & context. It emphasizes the reliability and interpretation of the data.
            - It also has Perceptive Design, as Boxplots are common statistical tools to present data with a range of values and hence quite intuitive to the stakeholders. It holds true for the Stacked Bar Chart as well. Both visualizations have a clear, standardized visual hierarchy.
            - Aesthetic design emphasizes visual appeal and pleasantness. The Boxplot is fairly plain but the Stacked Bar Chart is quite visualling appealing.
            - The Excel Line Chart shows the temporal trend of outbreaks over time, whereas the Bar Chart shows the number of outbreaks by type of outbreaks. Both are very intuitive & easy to interpret.


    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization? 

        - To ensure reproducibility, the followings are used & hereby stated:
            - Raw data: dataset used to generate the visualization is accessible for verification
            - Audit trail: comments within the Python code to explain each part of the process & methodology
            - Version Control: via GitHub
            - Executable codes: from start to finish
            - Reproducible Environment: The Python code runs in a consistent environment i.e. DSI_participant (Python 3.9.20)
            - Excel is run in Microsoft Excel for Mac Version 16.94 (25020927) where the plots generated can easily be duplicated

        - Consequences of the lack of reproducibility: 
            - Reduced credibility, accuracy, & transparency 
            - Error-prone analysis & ineffective decision-making with operational, strategic, & financial implications 
            - Not conducive to collaborative work & future updates
            
    
    > How did you ensure that your data visualization is accessible?  

            - Color Accessibility - for the Box plot, it is color-blind friendly; for the Stacked Bar Chart, with the multi-color nature, it is challenging to make it color-blind friendly without making it harder to read for the non-colorblind
            - Clear and Readable Fonts - size of fonts increased & bolded for axis titles
            - High Contrast between text/plots and background where possible i.e. dark against white background
            - Meaningful & descriptive titles with contextual information that explain what the data is showing
            - Use of Legends and Labels i.e. Stacked Bar Chart with clear legends & labels
            - The colors used in my Excel plots (line chart & bar chart) are Blue & Black with high contrast, are color-blind friendly as well. The fonts are good size and bolded for clarity.
        
    > Who are the individuals and communities who might be impacted by your visualization?  
        
        -Direct Impact:
            - Infection Prevention and Control practitioners
            - Public Health Officials 
            - Government Policy Makers
            - Healthcare Providers (Hospitals, Clinics, Doctors)
            - Epidemiologists
        
        -Indirect Impact:
            - The public & taxpayers
            - Family, friends & visitors of healthcare facilities residents


    > How did you choose which features of your chosen dataset to include or exclude from your visualization?

        -Features to include:
            - Relevance is the keyword. 
            - Duration of outbreak (time lapse between Outbreak begin to end), Number of Outbreaks, Causative Agent-1 & Outbreak Setting (type of facilities) are highly relevant from a public health perspective as they have infection prevention & control (patient isolation, use of personal protective equipment), strategic (e.g. vaccination campaigns, public awareness, sourcing of medications & vaccines, social distancing) & financial & resource implications
            - other visualizations that add value e.g. time series line graph - monthly outbreaks to indicate the seasonal nature i.e. maximum number of outbreaks during December & January, type of caussative agent during outbreaks etc.

        -Features to exclude:
            - Irrelevant info like Address & Name of institutions is excluded (no significance) in the context of Box plot or Stacked Bar Chart 
            - Causative Agent-2 info is excluded because it is insignificant comparing to Causative Agent-1 due to its rare occurence


    > What ‘underwater labour’ contributed to your final data visualization product?
        
        -Exploratory data scanning/analysis: 
            - scan the Excel dataset and applying filters to delve deeper e.g. types of facilities, causative agents, 
            - to check what kind of data I am dealing with, any missing data, numerical vs. categorical, relevant & meaningful domain-specific info to include
            - what derived info is needed e.g. Convert date to datetime format for Outbreak Duration calculation, Outbreak Duration = Date Declared Over - Date Outbreak Began
            - review summary data e.g. total no. of outbreaks and in relation to facilities/causative agents before proceeding with data visualizations
            - to decide if I need to tap into some resources to perform the visualizations e.g. simple visualizations can be easily done by Excel without Python, whereas Python codes are sometimes challenging to write e.g. a couple of codes are difficult to write without help
        
        -Design considerations: 
            - to ensure the principal design is substantive to reflect relevant, factual, accurate info with clarity, type of data visualization to present while maintaining some decent perceptive & aesthetic appeal
        
        -Accessibility considerations:
            - codes changed to increase font size, bold fonts where needed, ensure colorblind-friendliness with monochrome i.e. Boxplot
        
        -Reproducibility considerations:
            - to ensure comments are made within the codes


- This assignment is intentionally open-ended - you are free to create static or dynamic data visualizations, maps, or whatever form of data visualization you think best communicates your information to your audience of choice! 
- Total word count should not exceed **(as a maximum) 1000 words** 
 
### Why am I doing this assignment?:  
- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes: 
* Create and customize data visualizations from start to finish in Python
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story  
- This would be a great project to include in your GitHub Portfolio – put in the effort to make it something worthy of showing prospective employers!

### Rubric:

| Component         | Scoring  | Requirement                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| Data Visualizations | Complete/Incomplete | - Data visualizations are distinct from each other<br>- Data visualizations are clearly identified<br>- Different sources/rationales (text with two images of data, if visualizations are labeled)<br>- High-quality visuals (high resolution and clear data)<br>- Data visualizations follow best practices of accessibility |
| Written Explanations | Complete/Incomplete | - All questions from assignment description are answered for each visualization<br>- Explanations are supported by course content or scholarly sources, where needed |
| Code              | Complete/Incomplete | - All code is included as an appendix with your final submissions<br>- Code is clearly commented and reproducible |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 09/03/2025`
* The branch name for your repo should be: `assignment-4`
* What to submit for this assignment:
    * A folder/directory containing:
        * This file (assignment_3.md)
        * Two data visualizations 
        * Two markdown files for each both visualizations with their written descriptions.
        * Link to your dataset of choice.
        * Complete and commented code as an appendix (for your visualization made with Python, and for the other, if relevant) 
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-3`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
