---
layout: post
title: The House of Data Science
---

We have all seen Drew Conway's iconic Venn Diagram mapping out the facets of Data Science as a discipline.  Since 2013, when he presented the diagram, there have been various attempts at updating the diagram to further flesh out what makes up data science.  None of them really make describing the discipline any easier and if anything, has made the situation even more confusing for some (Data Science = Software Development).  They also don't make developing a curriculum for data science instruction or teaching the subject any easier.  To that end, here is my attempt at describing the discipline of data science shown in the picture below.


<img src="/images/DSHouse.png" style = "display: block; margin-left: auto;margin-right:auto;" width="400px" height="400px"/>

Data science, to me, seems more like a house with a roof, support columns and a foundation.  Each structural element symbolizes the three main components making up data science: Statistical Methods, Computing Tools (R, SQL and Python), and communication skills/domain knowledge. Let's describe this from the bottom up.

1. The Foundation - Statistical Methods
   
   **Statistics is the foundation of data science.** Everything that is done in data science is dependent on statistical methods. It doesn't matter whether you are focused on prediction or explanation, the code you are running on your computer is based on a statistical method that was developed a long time ago. Some examples of this are shown in the table below:

    <table><table style="float: center">
      <tr>
        <th>Statistical Method</th>
        <th>Development Date</th>
      </tr>
      <tr>
        <th>Linear Regression</th>
        <th>1795, 1805</th>
      </tr>
      <tr>
        <th>K-Means Clustering</th>
        <th>1957</th> 
      </tr>
      <tr>
        <th>Logistic Regression</th>
        <th>1958</th>
      </tr>
      <tr>
        <th>K-Nearest Neighbors</th>
        <th>1951-1967</th>
      </tr>
      <tr>
        <th>Rigde Regression</th>
        <th>1970</th>
      </tr>
      <tr>
        <th>Bootstrapping</th>
        <th>1979</th>
      </tr>
    </table>                        
                        
   The thing with many statistical methods is that they tend to be based on assumptions on how the data are distributed. Even those that are not (non-parametric methods) have limitations.  These limitations and assumptions can be easily missed by an untrained or novice analyst and can render any conclusions useless.  With the advent of statistical software and the influx of people who lack training in statistics coming into the profession, faulty analyses .  Add to this the idea that the "algorithm" can make sense of a bad experimental design and you have a data science house that is built on a foundation of sand with the inevitable collapse to follow.

2. The Columns- Computing Tools

   **This is the rightful place of computing.  In the center of the house.**  Code is essentially a communication medium, like writing, nothing more.  What computing tools do is similar to a what the load bearing columns do in a structure; support the roof and transfer the load from the roof to the foundation.  Within the realm of data science, mastery of computing tools allows the the analyst to be more efficient in analyzing data, analyze larger data sets, and more types of data.  Mastering computing tools also allows a data scientist to interact better with software developers and develop applications based on statistical methods.  On the flip side, not having good knowledge of computing tools such as Python, R and SQL is like having a home with weak columns. A structure with weak columns can't support the roof and makes it unstable.  The breath of problems you can solve is less and you are limited in how complex of a problem you can solve.

3. The Roof-Domain Knowledge and Communication Skills

   Domain knowledge and communication skills are like the roof of a structure in that a roof needs the columns and foundation in order for it to remain intact.  A solid roof also protects the columns and foundation from the outside elements and is the first element that a load encounters.  Likewise, domain knowledge is necessary in order to interpret the results of an analysis correctly.  It is also necessary at the beginning stages of a project in that the problem to be analyzed must be defined correctly so that the right data is collected and the appropriate analysis techniques are used.  

   Communication skills are needed so that the results of an analysis can be explained to a decision maker **in a way they can understand** so that appropriate action can be taken based on the analysis results.  This could be in the form of a written report or a PowerPoint presentation. Sometimes data scientists must give decision makers bad news based on an analysis or propose improvement ideas that may not be popular with portions of a company.  This requires large amounts of diplomacy and tact which only comes with good communication skills and experience.  On the front end of a project, effective communication is needed in order to propose analysis projects and negotiate the scope of the project.  It also is important within the scope of a project team.  Good communication skills also can diffuse any group dynamics issues that can arrise during a project.

   So what does a lack of domain knowledge or communication skills give you?  A lack of domain knowledge can result in solving the wrong problem using the wrong tools. Or it can lead to collecting too much data, not enough data or the wrong data. It can also lead to incorrectly interpreting the results of an analysis resulting in bad decisions by management.  Either way, this can put a data scientist's (or a data science team's)credibility in question.  Given the salaries that data scientists can command, this can have bad consequences.  

   Lack of communication skills can also result in the loss of credibility since, if a non-technical manager can't understand the results of an analysis, they won't use the information.  This can lead management to question the value of a data science group (Again think $$ here). **The value a data scientist brings is in the insight they provide.** Not having good communication skills is also career-limiting for an individual data scientist.  **The higher you move up in a company, the more communication skills are needed.  Good businesses value people, ideas and things. In that order. A data scientist that can't communicate effectively will not be trusted with more responsibility.**

   One thing to realize in looking at data science as a house is that it also shows one path for how data scientists can learn the discipline and progress in their career.  Step 1 is learning statistics.  Step 2 is developing programming skills. First as a user then developing to the point(if so desired) where production level code can be written. Step 3. is acquiring domain knowledge and developing communication skills.  In my view, this makes sense from a teaching perspective and from the standpoint of career development.
