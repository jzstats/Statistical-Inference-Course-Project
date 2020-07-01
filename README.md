About The Assignment
====================

This project was created for the peer-graded assignment of:

> Course 6: Statistical Inference,  
> from Data Science Specialization,  
> by Johns Hopkins University,  
> at Coursera

The course is taught by:

-   Jeff Leek, PhD  
-   Roger D. Peng, PhD  
-   Brian Caffo, PhD

The assignment consists of 2 parts:  

1. Simulation Exercise  
2. Basic Inferential Data Analysis  

As putted by the teachers of the course, for the Part 1: 

> **Part 1: Simulation Exercise Instructions**  
> 
> In this project you will investigate the exponential distribution in R and compare it with the Central Limit Theorem. The exponential distribution can be simulated in R with rexp(n, lambda) where lambda is the rate parameter. The mean of exponential distribution is 1/lambda and the standard deviation is also 1/lambda. Set lambda = 0.2 for all of the simulations. You will investigate the distribution of averages of 40 exponentials. Note that you will need to do a thousand simulations.
> 
> Illustrate via simulation and associated explanatory text the properties of the distribution of the mean of 40 exponentials. You should
>
> 1. Show the sample mean and compare it to the theoretical mean of the distribution.
> 2. Show how variable the sample is (via variance) and compare it to the theoretical variance of the distribution.
> 3. Show that the distribution is approximately normal.
> 
> In point 3, focus on the difference between the distribution of a large collection of random exponentials and the distribution of a large collection of averages of 40 exponentials.
> 

Respectively for the Part 2:  

> **Part 2: Basic Inferential Data Analysis Instructions**
>
> Now in the second portion of the project, we're going to analyze the ToothGrowth data in the R datasets package.
> 
> 1. Load the ToothGrowth data and perform some basic exploratory data analyses
> 2. Provide a basic summary of the data.
> 3. Use confidence intervals and/or hypothesis tests to compare tooth growth by supp and dose. (Only use the techniques from class, even if there's other approaches worth considering)
> 4. State your conclusions and the assumptions needed for your conclusions.

Both parts must comform to the supplied directions:  

> You will create a report to answer the questions. Given the nature of the series, ideally you'll use knitr to create the reports and convert to a pdf. (I will post a very simple introduction to knitr). However, feel free to use whatever software that you would like to create your pdf.
>
> Each pdf report should be no more than 3 pages with 3 pages of supporting appendix material if needed (code, figures, etcetera).

According to the instruction of the assignment, 2 PDFs that were produced:  

1. [simulation_exercise.pdf](https://github.com/jzstats/Statistical-Inference-Course-Project/blob/master/simulation_exercise/simulation_exercise.pdf), that can be found at the directory *simulation_exercise*   
2. [basic_inferential_data_analysis.pdf](https://github.com/jzstats/Statistical-Inference-Course-Project/blob/master/basic_inferential_data_analysis/basic_inferential_data_analysis.pdf), that can be found at the directory *basic_inferential_data_analysis*  

Each of these directories contains the corresponding .Rmd file that was compiled to produce each pdf as well as supplementary files that were automatically created as part of the selected template, *Association for Computing Machinery* from 'rticles' package. 

Some minor adjustement were made manually to the original template *acm_proc_article-sp.cls*:  

1. At the line 781 the following change was made for both *simulation_exercise/acm_proc_article-sp.cls* 
and *basic_inferential_data_analysis/acm_proc_article-sp.cls*:   
     > \section*{ABSTRACT}\normalsize %\the\parskip \the\baselineskip%\ninept  
     
   replaced with  
     > \section*{OVERVIEW}\normalsize %\the\parskip \the\baselineskip%\ninept  
   
   in order to display OVERVIEW instead of ABSTRACT as the title of first section in the pdf outputs.  
2. The space reserved for the ACM Copyright Notice, was used instead of its intented porpose (that is to contain a Copyright Notice), 
   to host a custom notice that leads to the corresponding directory of this GitHub repository 
   that contains all the supplementary information and files that were used to produce each report. 
   To do this between the lines 1457 and 1458, the following code chunks were added:  
   at the *simulation_exercise/acm_proc_article-sp.cls*:  
     > % Added a custom notice in place of the ACM Copyright Notice.  
     > \toappearbox{  
     >   \underline{SUPPLEMENTARY INFORMATION}  
     >   \newline  
     >   Further details can be found at the GitHub repository:  
     >   \newline  
     >    \url{https://github.com/jzstats/Statistical-Inference-Course-Project/simulation_exercise}  
     > }  
     
   at the *basic_inferential_data_analysis/acm_proc_article-sp.cls*:  
     > % Added a custom notice in place of the ACM Copyright Notice.  
     > \toappearbox{  
     >   \underline{SUPPLEMENTARY INFORMATION}  
     >   \newline  
     >   Further details can be found at the GitHub repository:  
     >   \newline  
     >    \url{https://github.com/jzstats/Statistical-Inference-Course-Project/basic_inferential_data_analysis}  
     > }  
    
3. The code in line 839:  
     > \begin{picture}(20,6) %Space for copyright notice  
     
   at the *basic_inferential_data_analysis/acm_proc_article-sp.cls* it was replaced with:    
     > \begin{picture}(20,3) %Space for copyright notice  
     
   in order to shrink the space reserved for the AMC Copyright Notice.  
4. The references were created manually for both pdfs and the files that could automatically produce them were ignored. 
