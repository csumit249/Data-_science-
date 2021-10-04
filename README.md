# Data-Science
## Introduction to Data Science
 Data Science is a blend of various tools, algorithms, and machine learning principles with the goal to discover hidden patterns from the raw data. 
Data Science is primarily used to make decisions and predictions making use of predictive causal analytics, prescriptive analytics (predictive plus decision science) and machine learning.

  ![image](https://user-images.githubusercontent.com/42414598/134496371-e86db33d-1b05-4594-b6d0-894525ff3368.png)

  
  # <h1> Data Science Goals and deliverables
* Prediction (predict a value based on inputs)
* Classification (e.g., spam or not spam)
* Recommendations (e.g., Amazon and Netflix recommendations)
* Pattern detection and grouping (e.g., classification without known classes)
* Anomaly detection (e.g., fraud detection)
* Recognition (image, text, audio, video, facial, …)
* Actionable insights (via dashboards, reports, visualizations, …)
* Automated processes and decision-making (e.g., credit card approval)
* Scoring and ranking (e.g., FICO score)
* Segmentation (e.g., demographic-based marketing)
* Optimization (e.g., risk management)
* Forecasts (e.g., sales and revenue)
 
  ![image](https://user-images.githubusercontent.com/42414598/134496834-ae37c336-6549-4697-87e2-8361172ae688.png)
  
# <h1> Business Intelligence (BI) vs. Data Science : 
    
  ![image](https://user-images.githubusercontent.com/42414598/134497111-83a95e8e-ad1b-4a5a-b07e-208c77b7cd2e.png)

# <h1> Data Science
     
Phase 1—The required resources present in terms of people, technology, time and data to support the project. In this phase, you also need to frame the business problem and formulate initial hypotheses (IH) to test.
Data preparation: You need to explore, preprocess and condition data prior to modeling. Further, you will perform ETLT (extract, transform, load and transform) to get data into the sandbox. Let’s have a look at the Statistical Analysis flow below

![Untitled-1](https://user-images.githubusercontent.com/42414598/134766825-a49c2b3a-bb84-4f2a-8ca9-3eda56ed35df.jpg)
 
# <h1> Model Planning 
  
 We will determine the methods and techniques to draw
 the relationships between variables. These relationships
 will set the base for the algorithms which you will 
Implement in the next phase. You will apply Exploratory
 Data Analytics (EDA) using various statistical formulas and visualization tools.
* __R__ has a complete set of modeling capabilities and 
provides a good environment for building interpretive 
models.
* __SQL Analysis services__ can perform in-database
 analytics using common data mining functions and 
basic predictive models.
* __SAS/ACCESS__  can be used to access data from
Hadoop and is used for creating repeatable and reusable 
model flow diagrams. Although, many tools are present 
in the market but R is the most commonly used tool

![2 (1)](https://user-images.githubusercontent.com/42414598/134766838-6d811ae2-14ac-4a27-91de-8b5926590048.jpg)

      
# <h1> Statistics and Visualization
 
 Statistics is a mathematical science that is concerned with the collection, analysis, interpretation or explanation,and presentation of data. Properly used statistical principles are essential in guiding any inquiry informed by data and,especially in the phase of data exploration, is routinely a fundamental source for discovery and innovation. Insights
from data may come from a well conceived visualization of the data, from modern methods of statistical learning and model selection as well as from time-honored formal statistical procedures.
 
 # <h1> Displaying Data
 The first encounters one has to data are through graphical displays and numerical summaries. The goal is to find an elegant method for this presentation that is at the same time both objective and informative - making clear with a few lines or a few numbers the salient features of the data. In this sense, data presentation is at the same time an art, a
science, and an obligation to impartiality.
 
 
 Types of Data
 A data set provides information about a group of individuals.
 • Individuals are the objects described by the data.
 • Variables are characteristics of an individual. In order to present data, we must first recognize the types of data under consideration.
       – Categorical variables partition the individuals into classes. Other names for categorical variables are levels or factors. One special type of categorical variables are ordered categorical variables that suggest a ranking, say small. medium, large or mild, moderate, severe.
      – Quantitative variables are those for which arithmetic operations like addition and differences make sense.
 
 Example 1.1 (individuals and variables). We consider two populations - the first is the nations of the world and the second is the people who live in those countries. Below is a collection of variables that might be used to study these populations.
 
 nations-         people
 
population size-  age
 
time zones-       height
 
average rainfall- gender
 
life expectancy-  ethnicities
 
mean income-      annual income
 
literacy rate-    literacy
 
capital city-     mother’s maiden name
 
largest river-    marital status
 
 
# <h1> Categorical Data

 Pie Chart
 A pie chart is a circular chart divided into sectors, illustrating relative magnitudes in frequencies or percents. In a pie chart, the area is proportional to the quantity it represents.
 
 ![image](https://user-images.githubusercontent.com/42414598/135810376-89916b8c-d988-4276-89a4-2eb45bc9027e.png)

 Gene Ontology
    (GO) project is a bioinformatics initiative whose goal is to provide unified terminology of genes and their products. The project began in 1998 as a collaboration between three model organism databases, Drosophila, yeast, and mouse. The GO Consortium presently includes many databases, spanning repositories for plant, animal and microbial genomes. This project is supported by National Human Genome Research Institute. 
 ![image](https://user-images.githubusercontent.com/42414598/135810536-56844108-14a7-43df-9f63-29c4aeb17b05.png)
 
 To make a simple pie chart in Rfor the proportion of AIDS cases among US males by transmission category.
> males<- c(58,18,16,7,1)
> pie(males)
 
 • Define some colors ideal for black and white print.
> colors <- c("white","grey70","grey90","grey50","black")
            
• Calculate the percentage for each category.
> male_labels <- round(males/sum(males)*100, 1)
The number 1 indicates rounded to one decimal place.
> male_labels <- paste(male_labels, "\%", sep=" ")
This adds a space and a percent sign.
                 
• Create a pie chart with defined heading and custom colors and labels and create a legend.
> pie(males, main="Proportion of AIDS Cases among Males by Transmission Category
+ Diagnosed - USA, 2005", col=colors, labels=male_labels, cex=0.8)
> legend("topright", c("Male-male contact","Injection drug use (IDU)",
+ "High-risk heterosexual contact","Male-male contact and IDU","Other"),
+ cex=0.8,fill=colors)

# <h1> Bar Charts
 The human eye is good at judging linear measures and poor at judging relative areas, a bar chart or bar graph is often preferable to pie charts as a way to display categorical data.
To make a simple bar graph in R,
> barplot(males)
 
 • Enter the data for females and create a 5 ×2 array.
> females <- c(0,71,27,0,2)
> hiv<-array(c(males,females), dim=c(5,2))
                               
# <h1> Two-way Tables   
 Relationships between two categorical variables can be shown through a two-way table (also known as a contingency table , cross tabulation table or a cross classifying table ).
 
Example . In 1964, Surgeon General Dr. Luther Leonidas Terry published a landmark report saying that smoking may be hazardous to health. This led to many influential reports on the topic, including the study of the smoking habits of 5375 high school children in Tucson in 1967. Here is a two-way table summarizing some of the results.
 
 ![image](https://user-images.githubusercontent.com/42414598/135822386-47fcecd8-dcc6-45a8-9f1e-8b6ec616639b.png)
• The row variable is the parents smoking habits.
• The column variable is the student smoking habits.
• The cells display the counts for each of the categories of row and column variables.
 
 
 # <h1> Histograms and the Empirical Cumulative Distribution Function
 Histograms are a common visual representation of a quantitative variable. Histograms summarize the data using rectangles to display either frequencies or proportions as normalized frequencies. In making a histogram, we   
  • Divide the range of data into bins of equal width (usually, but not always). 
  
  • Count the number of observations in each class. 
  
  • Draw the histogram rectangles representing frequencies or percents by area.
  
Interpret the histogram by giving 
  
  • the overall pattern
  
  – the center
  – the spread
  – the shape (symmetry, skewness, peaks)
  • and deviations from the pattern
  – outliers
  – gaps
  
