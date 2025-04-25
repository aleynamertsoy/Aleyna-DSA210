# TikTok Usage Analysis: Trends, Patterns, and User Behavior

## Motivation
TikTok is one of the most widely used social media platforms, and I have always been curious about how it influences my daily routines, attention span, and content preferences. With this project, I aim to take a data-driven look at my own usage patterns. By analyzing my watch history data, I want to better understand how my interactions with the platform evolve over time and how different factors influence my engagement levels.

## Dataset and Source
The dataset is downloaded directly from the TikTok app using the official data request feature. It is provided in JSON format and includes:
- Timestamped watch history
- Video metadata (when available)
- Device information and other relevant metadata

## Data Enhancement Strategy
To transform the raw data into something meaningful, I will add several new dimensions to enrich the analysis:
- **Day of the Week**: For understanding behavioral patterns across weekdays and weekends.
- **Time of Day**: Categorizing watch timestamps into Morning, Afternoon, Evening, and Night.
- **Session Grouping**: Estimating continuous usage periods as sessions to analyze binge-watching behavior.
- **Academic Calendar Context**: I will integrate my university's academic calendar to flag national holidays and semester breaks, allowing me to evaluate whether holidays lead to increased screen time.

## Planned Analysis Workflow
1. **Preprocessing and Feature Engineering**
   - Parse JSON data into structured format (Pandas DataFrame)
   - Generate enriched features (e.g., time bins, sessions, holiday flagging)
   
2. **Exploratory Data Analysis (EDA)**
   - Analyze peak viewing times and weekly patterns
   - Visualize frequency of different session lengths
   - Detect spikes in usage around holiday periods

3. **Statistical Testing**
   - Use t-tests or ANOVA to evaluate if watch durations differ significantly between regular days and holidays
   - Analyze category-specific viewing shifts over time

4. **Machine Learning Application**
   - I plan to apply clustering (e.g., k-means) to group similar usage sessions
   - I will attempt time series modeling or classification to predict whether a given session is likely to happen on a holiday based on previous behavior patterns

## Deliverables
- Cleaned and enriched dataset derived from raw TikTok JSON
- Jupyter notebooks for EDA and modeling
- Visualizations summarizing key behavioral patterns
- A machine learning model and prediction results

## Notes
All work will be documented on GitHub, and regular commits will reflect the evolution of this project. Machine learning applications will be clearly explained with rationale for each step taken.
