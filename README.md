# School_District_Analysis

## Overview of Prject

The purpose of this project was to gain better understanding of Python, and to gain a basic understanding of numpy and pandas.  two libraries in pytohon that help you read and 
manipulate .csv files or "comma separated variable' files. To complete this challenge and module we had to have an understanding of how to read and write to .csv files, how to 
use pandas and numpy to better read and manipulate the data. Using those same libaries, we also manage to analyze the data and come to results about them. Lastly, we corrected data that was later fvound out to be fradulent and disqualified it from the analyis. As always we then took those results and put them into a format that is easily accessible. 

## Results 

 - Removing the fradulent data caused the percent passing of math, reading and overall to go down in the district summary. This is excepted if fradulent scores were removed. 
 - Most of the schools in the school summary were not changed, the difference as seen below :
 
 Pre Removal
![Pre removal](https://github.com/HussanK/School_District_Analysis/blob/main/fgi3.png)
 Post Removal
 ![Post removal](https://github.com/HussanK/School_District_Analysis/blob/main/fig2.png)

As you can see all of the passing percentages went down. 
 
 -  Thomas high's placement isn't actaully changed when removing all of the 9th grade scores. 
 To remove the ninth graders from Thomas High we used this code:

```
school_data_complete_df.loc[(school_data_complete_df['school_name']=='Thomas High School') & (school_data_complete_df['grade']!='9th')]
```
This bit of code looks for anyone from Thomas High School, whose grade is not 9th. 

 - By removing the ninth graders from Thomas High, the percent passing for 9th grades went down. 
 - By removing the ninth graders from Thomas High, the percent passing of all schools spending 630-644 on each student stayed the same 
 - By removing the ninth graders from Thomas High, the percent passing of all medium sized schools was unchanged
 - By removing the ninth graders from Thomas High, the percentage passing of all Charter schools was also unchanged
 
 ## School_Data_Analysis Summary
 
 Four changes that removing the 9th graders from Thomas High School made were, the percentage passing of 9th graders went down, as Thomas High School maintains an high average 
 passing percent. The overall passing percent went down, as again Thomas High School was ranked highly in overall passing percent. The reading passing rate went down. Lastly, 
 the math passing percent went down.  
 
