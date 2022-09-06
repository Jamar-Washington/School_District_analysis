# School_District_analysis

## Project Overview
In the PyCitySchools project, we are helping Maria, who is the chief data scientist for a city school district, with looking at trends from standarized testing.
That way, the schools and the school district can best determine what changes need to be addressed in the future. 
Using Jupyter Notebook, we are able to look at the data regarding math and reading scores, schools that the students go to, as well as the budget that each student 
recieves.
With that data, we are able to make an analysis based on the school's spending, size, and type to see how they differ.

## Results

* How is the district summary affected?

Since the only thing that was changed was replacing the ninth graders' grades, there was no major changes to the distict summary as 14 schools 
had no changes to their data. The only change is the Thomas High School data.

* How is the school summary affected?

In the Thomas High School summary, the average score dropped in math but rose in reading. However, the overall score dropped over 
.3 percent as seen at the end of the image.

![ThomasChange](https://user-images.githubusercontent.com/109183214/188536969-cb828dbb-3613-4cf8-90a2-0e4f4a398660.png)
![Thomas](https://user-images.githubusercontent.com/109183214/188536968-a376fc5d-746c-4783-9100-6a9264f2274a.png)
  
* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Thomas High School's performance relative to the other schools was mostly unchanged. They were still second best overall in passing rate. However, since 
Thomas High had a worse overall passing percentage, the difference between Thomas and Griffin High went from about .35 percent to about .03 percent.
![Head](https://user-images.githubusercontent.com/109183214/188536100-adb4563c-c1b0-4be8-977d-c136a2408310.png)
![HeadChange](https://user-images.githubusercontent.com/109183214/188536101-87d80d8f-af7d-4d51-b9eb-815d11a531f6.png)

* How does replacing the ninth-grade scores affect the following:

  * Math and reading scores by grade
  
  In the math scores, the only thing that changed was the ninth grade changing from a number to NaN as seen below.
  
  ![MathbyGrade](https://user-images.githubusercontent.com/109183214/188535451-31008ae2-f0a1-4634-adab-0d4c91ed5df8.png)
  ![MathbyGradeChange](https://user-images.githubusercontent.com/109183214/188535453-e2ae66d3-5562-41ae-8a25-00f68b31eec9.png)

  That is a similar case with the reading scores below.
  
  ![ReadingbyGrade](https://user-images.githubusercontent.com/109183214/188535408-3da2a646-cef6-41eb-804a-0729221eddfa.png)
  ![ReadingbyGradeChange](https://user-images.githubusercontent.com/109183214/188535406-73562bb2-b301-4391-8778-3a6b3d7e0ea5.png)

  * Scores by school spending
  ![ScorebySpending](https://user-images.githubusercontent.com/109183214/188530229-855bb920-096b-4525-9522-b60385a3d7b3.png)
  ![ScorebySpendingChange](https://user-images.githubusercontent.com/109183214/188530230-0378c05d-f76d-408e-80e4-976c724c723f.png)

  * Scores by school size
  ![ScorebySize](https://user-images.githubusercontent.com/109183214/188530283-310f3b8f-6471-4db6-b63c-1fcd4fe28de3.png)
  ![ScorebySizeChange](https://user-images.githubusercontent.com/109183214/188530280-96bf1dac-33a1-4cc0-84e7-0b92cfe5efd7.png)

  * Scores by school type
  ![ScorebyType](https://user-images.githubusercontent.com/109183214/188530307-802c1670-71bb-4a34-9f8b-7bfb48546738.png)
  ![ScorebyTypeChange](https://user-images.githubusercontent.com/109183214/188530308-0c8398a3-1c4a-41ad-a594-6d0118abb5a8.png)

 With the scores filtered by spending, size, and type, there was no difference in overall passing. One noticable change that percentages of passing in math and reading
 alone did increase a lot. This could mean that the NaN was affected the calculations when looking at the subjects as some student's grade may have had a NaN in one
 subject but not the other.
 
## Summary
In summary, with the changing of the ninth graders' grade to NaN, there was a change to the average math and reading scores at Thomas High. This is because the NaN grades
were not accounted for in the average score. Also, the percentage of math, reading, and overall passing changed. That is due to the fact that when the grades were 
changed to NaN, we excluded ninth graders from the total count of students that were graded, changing the denominator in the percentage calculations.
