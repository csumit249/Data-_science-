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
 
 
![image](https://user-images.githubusercontent.com/42414598/135840290-975b1478-bbd5-41d4-896c-1594288dc063.png)
 
 
 
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
  
 # <h1> Scatterplots
 
 We now consider two dimensional data. The values of the first variable x1,x2,...,xn are assumed known and in an experiment and are often set by the experimenter. This variable is called the explanatory, predictor, discriptor, or input variables and in a two dimensional scatterplot of the data display its values on the horizontal axis. The values
y1,y2 ...,yn, taken from observations with input x1,x2,...,xn are called the response or target variable and its values are displayed on the vertical axis. In describing a scatterplot, take into consideration 
 
 • the form, for example,
 
 – linear
 
– curved relationships
 
 – clusters
 
 • the direction,
 
 – a positive or negative association
 
 • and the strength of the aspects of the scatterplot.
 
 Example 1.17 (Fossils of the Archeopteryx). The name Archeopteryx derives from the ancient Greek meaning “ancient feather” or “ancient wing”. Archeopteryx is generally accepted by palaeontologists as being the oldest known bird. Archaeopteryx lived in the Late Jurassic Period around 150 million years ago, in what is now southern Germany
during a time when Europe was an archipelago of islands in a shallow warm tropical sea. The first complete specimen of Archaeopteryx was announced in 1861, only two years after Charles Darwin published On the Origin of Species,and thus became a key piece of evidence in the debate over evolution. Below are the lengths in centimeters of the femur and humerus for the five specimens of Archeopteryx that have preserved both bones.
 
 
 ![image](https://user-images.githubusercontent.com/42414598/135827166-12d719e1-120e-49b8-a014-8d67a2d83903.png)

 
 # <h1>  Time Plots
 
 
 Some data sets come with an order of events, say ordered by time.
 
Example 1.19. The modern history of petroleum began in the 19th century with the refining of kerosene from crude oil. The world’s first commercial oil wells were drilled in the 1850s in Poland and in Romania.The first oil well in North America was in Oil Springs, Ontario, Canada in 1858. The US petroleum industry began with Edwin Drake’s drilling
of a 69-foot deep oil well in 1859 on Oil Creek near Titusville, Pennsylvania for the Seneca Oil Company. The industry grew through the 1800s, driven by the demand for kerosene and oil lamps. The introduction of the internal combustion engine in the early part of the 20th century provided a demand that has largely sustained the industry to this day.
Today, about 90% of vehicular fuel needs are met by oil. Petroleum also makes up 40% of total energy consumption in the United States, but is responsible for only 2% of electricity generation. Oil use increased exponentially until the world oil crises of the 1970s.
 
 ![image](https://user-images.githubusercontent.com/42414598/135827409-0d8a9ec0-b8ed-4dd1-b576-b1927bd41c4c.png)
 
 
 With the data given in two columns oil and year, the time plot plot(year,oil,type="b") is given on the left side of the figure below. This uses type="b" that puts both lines and circles on the plot.
 
 ![image](https://user-images.githubusercontent.com/42414598/135827519-5d82f524-a9e4-4afe-b881-17126284aec1.png)
 

 
 Sometimes a transformation of the data can reveal the structure of the time series. For example, if we wish to examine an exponential increase displayed in the oil production plot, then we can take the base 10 logarithm of the production and give its time series plot. This is shown in the plot on the right above. (In R, we write log(x) for the natural logarithm and log(x,10) for the base 10 logarithm.
 
 # <h1> Chapter 2 Describing Distributions with Numbers
 
 These data can be subject to the operations of arithmetic.In particular, we can add or subtract observation values, we can sort them and rank them from lowest to highest.
We will look at two fundamental properties of these observations. The first is a measure of the center value for the data, i.e., the median or the mean.
 
In addition, to give a sense of the spread in the data, we often give the smallest and largest observations as well as the observed value that is 1/4 and 3/4 of the way up this list, known at the first and third quartiles. This difference, known as the interquartile range is a measure of the spread or the dispersion of the data. For the mean, we commonly use the standard deviation to describe the spread of the data.
 
 1 Medians
 
 The median take the middle value for x1,x2,...,xn after the data has been sorted from smallest to largest, x(1),x(2),...,x(n).
 (x(k) is called the k-th order statistic. Sorting can be accomplished in Rby using the sort command.) If n is odd, then this is just the value of the middle observation x((n+1)/2). If n is even, then the two values closest to the center are averaged. 
 
![image](https://user-images.githubusercontent.com/42414598/135830687-2785fab4-9c57-4c89-b381-98df7db96b7a.png)
 
 2 Means
 
 For a collection of numeric data, x1,x2,...,xn, the sample mean is the numerical average.
 
 ![image](https://user-images.githubusercontent.com/42414598/135830894-dfce3f46-e1b4-4948-935b-6749325ae5ab.png)
 
Alternatively, if the value x occurs n(x) times in the data, then use the distributive property to see that So the mean  ̄x depends only on the proportion of observations p(x) for each value of x.
 
 ![image](https://user-images.githubusercontent.com/42414598/135831016-6c62805b-3840-4c40-adb6-e28ea860bf51.png)

 Example 2.1. For the data set {1,2,2,2,3,3,4,4,4,5}, we have n = 10 and the sum 
 1 + 2 + 2 + 2 + 3 + 3 + 4 + 4 + 4 + 5 = 1n(1) + 2n(2) + 3n(3) + 4n(4) + 5n(5)
       = 1(1) + 2(3) + 3(2) + 4(3) + 5(1) 
       = 30
Thus,  ̄x = 30/10 = 3.
 
 
 Example 2.2. For the data on the length in microns of wild type Bacillus subtilis data, we have
 ![image](https://user-images.githubusercontent.com/42414598/135831762-fcf6906a-49fe-4fcb-850b-be9a2a52e8da.png)
 
 So the sample mean  ̄x = 2.49.
If we store the data in Rin a vector x, we can write mean(x) which is equal to sum(x)/length(x) to
compute the mean. To extend this idea a bit, we can take a real-valued function hand instead consider the observations h(x1),h(x2),...,h(xn),
then
 ![image](https://user-images.githubusercontent.com/42414598/135831878-f9f38d17-2af9-42ae-be17-78d1618e8ed9.png)
 
# <h1> Five Number Summary
 
The first and third quartile, Q1 and Q3, are, respectively, the median of the lower half and the upper half of the data. The five number summary of the data are the values of the minimum, Q1, the median, Q3 and the maximum. Thesevalues, along with the mean, are given in Rusing summary(x).
 
 
 ![image](https://user-images.githubusercontent.com/42414598/135834015-768feac8-8e74-4fce-b2b6-76801bd094d5.png)

 
 We can display the five number summary using a boxplot.
> boxplot(age, main = c("Age of Presidents at the Time of Inauguration"))
 
 ![image](https://user-images.githubusercontent.com/42414598/135835647-f747b032-3d1c-4c3d-9f40-2d0aad5194f3.png)
 
 
 The value Q3 −Q1 is called the interquartile range and is denoted by IQR. It is found in Rwith the command IQR. Outliers are somewhat arbitrarily chosen to be those above Q3 + 3/2 IQR and below Q1 − 3/2 IQR. With this criterion, the ages of Ronald Reagan and Donald Trump, considered outliers, are displayed by the two circles at the top of the boxplot. The boxplot command has the default value range = 1.5 in the choice of displaying outliers. This can be altered to loosen or tighten this criterion.
 
 
 1 Sample Variance and Standard Deviation
 
 The sample variance averages the square of the differences from the mean
 
 
 ![image](https://user-images.githubusercontent.com/42414598/135836755-0b9f0e01-c504-41a2-936b-3ceeaaa9f739.png)
 

 Example 2.7. For the data set on Bacillus subtilis data, we have  ̄x = 498/200 = 2.49

 ![image](https://user-images.githubusercontent.com/42414598/135836921-3486f6f4-671e-40dd-8d51-905158e85e4f.png)

 So the sample variance s2x = 90.48/199 = 0.4546734 and standard deviation sx = 0.6742947. To accomplish this in R.

 ![image](https://user-images.githubusercontent.com/42414598/135837043-ba0b3f41-2ee1-4b76-a060-94f4071f922c.png)

 For quantitative variables that take on positive values, we can take the ratio of the standard deviation to the mean called the coefficient of variation as a measure of the relative variability of the observations. Note that cvx is a pure number and has no units.
 cvx = sx/ ̄x .
 
 ![image](https://user-images.githubusercontent.com/42414598/135837223-a69d1075-0156-45be-93ef-69a96d655f69.png)
  
2 Quantiles and Standardized Variables
 
 A single observation, say 87 on a exam, gives little information about the performance on the exam. One way to include more about this observation would be to give the value of the empirical cumulative distribution function.

 Exercise 2. For the example above, describe the quintile, decile, and percentile of the observation 87.
 
 
A second way to evaluate a score of 87 is to related it to the mean. Thus, if the mean  ̄x = 76. Then, we might say that the exam score is 11 points above the mean. If the scores are quite spread out, then 11 points above the mean is just a little above average. If the scores are quite tightly spread, then 11 points is quite a bit above average. Thus, for
comparisons, we will sometimes use the standardized version of xi, 
 
 ![image](https://user-images.githubusercontent.com/42414598/135839536-777bf087-71f7-4647-8129-369bfa5443a6.png)

 The observations zi have mean 0 and standard deviation 1. The value zi is also called the standard score , the z-value, the z-score, and the normal score. An individual z-score, zi, gives the number of standard deviations an observation xi is above (or below) the mean.
The R command scale transforms the data to the standard score. For the ages of the presidents, we use the scale command to show the standardized ages. The head command show the first 6 rows of the output for presidents from George Washington to John Qunicy Adams.
 
 ![image](https://user-images.githubusercontent.com/42414598/135839705-406c00fc-7881-40f1-95c9-7ca7277106b3.png)
 
 
# <h1> 3 Correlation and Regression
 
 Reflection soon made it clear to me that not only were the two new problems identical in principle with the old one of kinship which I had already solved, but that all three of them were no more than special cases of a much more general problem–namely, that of Correlation.
 
 1 Covariance and Correlation
 
 The covariance measures the linear relation-ship between a pair of quantitative measures x1,x2,...,xn and y1,y2,...,yn on the same sample of n individuals.
 
 ![image](https://user-images.githubusercontent.com/42414598/135992123-4b10eea1-57d7-454c-84d5-64be5b07dabb.png)

 
 ![image](https://user-images.githubusercontent.com/42414598/135992224-8308a1e2-8da1-4824-a08c-092e55e0c740.png)
 
 Exercise 1. Derive the alternative expression for the covariance:
 
 ![image](https://user-images.githubusercontent.com/42414598/135993113-5de44947-f15c-4513-8d86-2c7701565af2.png)

 Definition- The correlation, r, is the covariance of the standardized versions of x and y.
 
 ![image](https://user-images.githubusercontent.com/42414598/135993250-b337c1bd-1e0f-48fa-a02a-56309be1004a.png)
 
 The observations x and y are called uncorrelated if r(x,y) = 0.
 
 -> Linear Regression

 Covariance and correlation are measures of linear association. For the Archeopteryx measurements, we learn that the relationship in the length of the femur and the humerus is very nearly linear.  We now turn to situations in which the value of the first variable xi will be considered to be explanatory or predictive. The corresponding output observation yi, taken from the input xi, is called the response.
 
 me is the response.
In linear regression, the response variable is linearly related to the explanatory variable (also known as the co-variate), but is subject to deviation, discrepency, or to error. We write ![image](https://user-images.githubusercontent.com/42414598/135994906-d3c1f5e0-cb27-4108-b3b2-49be26e42be2.png)

 Example - Let’s begin with 6 points and derive by hand the equation for regression line.
 
 ![image](https://user-images.githubusercontent.com/42414598/135995144-7cc90980-6d62-4233-97ff-082bd7a77588.png)

 Add the x and y values and divide by n = 6 to see that  ̄x = 0.5 and  ̄y = 0.
 
 ![image](https://user-images.githubusercontent.com/42414598/135995263-192d2702-fd06-4daf-b6ad-370928399be1.png)

 Thus,
 ![image](https://user-images.githubusercontent.com/42414598/135995329-5c092e0f-9c14-4590-b80f-73beb0209831.png)

 As seen in this example, fits are rarely perfect. The difference between the fit and the data is an estimate ![image](https://user-images.githubusercontent.com/42414598/135995497-ca5fa9f1-e73c-46f3-97eb-a06612c20c42.png) for the error ![image](https://user-images.githubusercontent.com/42414598/135995519-fb8e6a04-64f0-4e84-bc54-74e3bb04f950.png) This difference is called the residual. So,
![image](https://user-images.githubusercontent.com/42414598/135995583-36643933-13a6-4989-bdaa-bd87bab8ce96.png)= RESIDUALi = DATAi −FITi = yi −ˆyi
 
 Exercise- Use the equation above to show that ![image](https://user-images.githubusercontent.com/42414598/135996032-9ed9c5ec-f064-4468-97f9-74808803e140.png)
 where the sums of squares of the fit or the variation of the fit,![image](https://user-images.githubusercontent.com/42414598/135996133-8a36b884-12a2-4cc0-b6a7-8e72c751f9fd.png)
 ,and the sums of squares of the data or the variation of the data,![image](https://user-images.githubusercontent.com/42414598/135996251-63620399-7603-4782-9105-3e771bf031c2.png)

 Because the fit and the residuals are uncorrelated, the Pythagorean identity (3.2) applies and we see that that
 
 ![image](https://user-images.githubusercontent.com/42414598/135996388-a87bde5e-9dd3-43b4-a4f9-3e649e520f28.png)

 This leads to the expression 
 ![image](https://user-images.githubusercontent.com/42414598/135996444-5b7104c2-e4c2-4e6f-85e7-272fd99b9772.png)

 where the sums of squares of the residuals or the variation of the residuals,
 ![image](https://user-images.githubusercontent.com/42414598/135996522-4351f007-feae-47b2-9943-0e0bac8beb85.png)
Thus, r2 of the variance in the data can be explained by the fit. As a consequence of this computation, many statistical software tools report r2 as a part of the linear regression analysis. For this reason, r2 is sometimes called the coefficient of determination. The remaining 1 −r2 of the variance in the data is found in the residuals.
 
  -> Transformed Variables
 
 For pairs of observations (x1,y1),...,(xn,yn), the linear relationship may exist not with these variables, but rather with transformation of the variables. In this case we have,
 
 ![image](https://user-images.githubusercontent.com/42414598/135996839-e2c145cf-40af-458a-ae40-489d2692bddc.png)

 A common choice to to perform linear regression on the variables  ̃y = g(y) and  ̃x = ψ(x) using the least squares criterion. In this case, g is called the link function
For example, if
 
 ![image](https://user-images.githubusercontent.com/42414598/135997073-dfbb0bd2-2db0-44cb-aa9d-9735d4cd8c04.png)
 
So, in (3.13), the link function g(yi) = ln yi. The parameters are α = ln A and β = k.Before we look at an example, let’s review a few basic properties of logarithms.
 
 Example- (Frank Amscombe). Consider the three data sets:
 
 ![image](https://user-images.githubusercontent.com/42414598/135997297-25b92169-322f-437e-90e9-51dea873f713.png)

 ![image](https://user-images.githubusercontent.com/42414598/135997382-1c9b0587-de95-452a-93c3-ee455435619b.png)

 Each of these data sets has a regression line ˆy = 3 + 0.5x and correlations between 0.806 and 0.816. However, only the first is a suitable data set for linear regression. This example is meant to emphasize the point that software will happily compute a regression line and an coefficient of determination value, but further examination of the data is required to see if this method is appropriate for any given data set.
 
 -> Extensions
 We will discuss briefly two extensions - the first is a least squares criterion between x and y that is nonlinear in the parameters β = (β0,...,βk). Thus, the model is
 ![image](https://user-images.githubusercontent.com/42414598/135997580-5cd2958b-8d3c-43c2-b80a-472e18afc1a8.png)

 for g, a nonlinear function of the parameters. The second considers situations with more than one explanatory variable.
 ![image](https://user-images.githubusercontent.com/42414598/135997641-634ec34d-646e-4e90-82ce-f48dbaf1d22d.png)
This brief discussion does not have the detail necessary to begin to use these methods. It serves primarily as an invitation to begin to consult resources that more fully develop these ideas.
 
 -> Nonlinear Regression
 
 Here, we continue using estimation of parameters using a least squares criterion.
 ![image](https://user-images.githubusercontent.com/42414598/135999258-0363630e-e3e8-4200-a38b-390071fdca74.png)
 
 For example, gradient descent (also known as steepest descent, or the method of steepest descent) is an iterative method in which produces a sequence of parameter values. The increment of the parameter values for an iteration is proportional to the negative of the gradient of SS(β) evaluated at the current point. The hope is that the sequence converges to give the desired minimum value for SS(β). 
 
 ![image](https://user-images.githubusercontent.com/42414598/135999889-57507486-9b9c-4821-ae2e-05e1c932ae70.png)
 
 -> Multiple Linear Regression
 
 Before we start with multiple linear regression, we first recall a couple of concepts and results from linear algebra.
• Let Cij denote the entry in the i-th row and j-th column of a matrix C.
• A matrix A with rA rows and cA and a matrix B with rB rows and cB columns can be multiplied to form a matrix AB provide that cA = rB, the number of columns in A equals the number of rows in B. In this case
 ![image](https://user-images.githubusercontent.com/42414598/136000042-3c86482c-3865-430f-b1d7-e13ed010e764.png)

 • The d-dimensional identity matrix I is the matrix with the value 1 for all entries on the diagonal (Ijj = 1,j =1 ...,d) and 0 for all other entries. Notice for and d-dimensional vector x, Ix = x.
• A d ×d matrix C is called invertible with inverse C−1 provided that CC−1 = C−1C = I.
Only one matrix can have this property.
• Suppose we have a d-dimensional vector a of known values and a d×d matrix C and we want to determine the vectors x that satisfy a = Cx.
This equation could have no solutions, a single solution, or an infinite number of solutions. If the matrix C is invertible, then we have a single solution x = C−1a.
• The transpose of a matrix is obtained by reversing the rows and columns of a matrix. We use a superscript T to indicate the transpose. Thus, the ij entry of a matrix C is the ji entry of its transpose, CT.
 
 Example->
 ![image](https://user-images.githubusercontent.com/42414598/136000320-011aad6a-f424-4a53-87b9-432525f37b63.png)
 
• A square matrix C is invertible if and only if its determinant det(C) not equal to 0. For a 2 ×2 matrix
 
 ![image](https://user-images.githubusercontent.com/42414598/136000524-9e1f4b9e-d5d9-4f8c-a56f-2867a98d644f.png)
 
 Example->  (ordinary least squares regression). In this case,
 
 ![image](https://user-images.githubusercontent.com/42414598/136000789-4f765fe5-165c-43ff-b8c6-227cdcb33859.png)

 ![image](https://user-images.githubusercontent.com/42414598/136000858-3665eb88-cb25-4b95-906b-56edb8935e8d.png)

 
