java c
STAT0045.   In-course Assessment 2   (2024/25 Session) 
Department of Statistical Science
General   Instructions 
· This assessment   is classified as Coursework as defined   in   the   UCL   Student   Regulations for   Exams and   Assessments.   It contributes 40% to the overall mark for this   module.
· The   release date for this assessment   is 12:00 (UK time) on Tuesday, 11 March 2025.
· The submission deadline   is 16:00 (UK time) on Tuesday, 18 March 2025.
· Individual extensions to the submission deadline can   only   be   granted where   a   student   has   been   issued with a Summary of Reasonable Adjustments (SoRA), has   used   a   Delayed Assessment            Permit (if the assessment is eligible), or   has   made   a valid   claim for   Extenuating   Circumstances.   The standard extension length for this assessment type   is five working days.
。 If you   have a SoRA, your extension should be setup   automatically   and   you   should   see   it
reflected   in the deadline displayed in the submission   portal.   If you think that your   SoRA
adjustment   has   not   been applied,   please contact the   module lead at the   earliest   opportunity.
。 Delayed   Assessment   Permits and   Extenuating Circumstances claims should be submitted   through   Portico. The   module lead will be notified and   will   act   on   extensions   approved   via         these   routes,   but the deadline displayed   in the submission portal will   not   update   instantly.
· In preparation for this assessment, please   ensure   that you   are   familiar with   the   Department   of   Statistical Science’s guidance on academic integrity. When   submitting your work, you   will   be         required to   make a declaration that you have   read and   understood this   guidance.
· Parts of your submission   may be scanned using   similarity   detection   software.   If any   breach   of the   assessment   regulations   is suspected,   it will   be   investigated   in accordance with   UCL’s Student
Academic   Misconduct   Procedure.
· To facilitate anonymous marking, you should not write your   name   anywhere   on   your work,
including   in file   names or file descriptions requested as part   of the   submission   process.
· You   must only submit your work via the designated   portal   in   Moodle.   If you try to submit via   email   or any other channel this will   not count as a   submission   and will   not   be   marked.
· There are strict, non-negotiable penalties for late   submission,   which   for   coursework   are   as   follows.
。 Up to 2 working days late: deduction   of   10   percentage   points,   but   no   lower than   the   pass   mark.
。 2-5 working days late: capped   at the   pass   mark.
。 More than 5 working days late:   mark   of   1.00%.
· If the   module lead becomes aware of a   significant   technical   issue   or   outage   affecting   Moodle
during the assessment, a message will be   circulated to   explain what   has   happened   and   the   steps      being taken to   mitigate the   issue.   If you do   not receive   notification of a more   widespread   issue   and   you experience technical difficulties, you should refer to the   Help      Support   resources   provided   by   UCL’s central   IT service.   However, last-minute technical   issues will   not be   considered   as valid
grounds for missing the deadline, so ensure that you   leave   plenty   of time to   prepare,   upload   and   check your submission.
· Non-submission (in the absence of any valid   Extenuating Circumstances)   will   mean   that   your
mark for this component   is   recorded as 0.00% and you will   be deemed   to   have   made   an   attempt.
· You should expect to receive feedback on this assessment   within   20   working   days   of the
submission deadline.   In the event of a delay, the module   lead   will   contact   students   directly   with   details of the revised timeline.
· ©2025   UCL. This assessment   paper is the   intellectual   property of UCL   and   subject to   copyright.   It   must   not   be   reproduced or shared with any third   party without   prior   permission of   UCL.
The assessment 
· This   is an individual assessment; you must work alone.
· This assessment consists of two parts.   For Part A, you can submit scanned/photographed   hand-   written solutions.   Make sure that scanned work can be   read   clearly.   Note the   UCL   advice   on submitting   scanned/photographed   work   (link(https://www.ucl.ac.uk/news/2020/apr/seven-simple- steps-submit-handwritten-answers-moodle-exams-or-assessments)).   For Part B you are required   to write a   report and this report should   be typed.   Include   a word   count for this   part. 
· The   relevant course   material for this assessment   is all the   material up to   and   including   Section
4.6.   Exercise Sheet 7   is not included.
· Keep your answers concise. Answers that are unnecessarily elaborate   or   include   information that   is   not asked for will be   penalised.
· Part   A and   Part   B are   both   marked on a scale 0-100,   and   are   equally weighted for the   final   mark.   For Part   A,   marks for the constituent   parts are listed   in   bold   face.   Marks   are   given   for   correct answers, but also for succinctness and clarity   of explanation.
· To ensure anonymous   marking, only   provide your Student   ID   number at the top   of   Part A and   B (and not your name).   Part A and   B should   be submitted together in one   PDF file. Submit   the   file with   your   Student   ID   as   name; for   example, if   your   ID   is   20001234,   use   the   name      20001234.pdf   .
· You can   use   R for the questions   in   Part A,   but do not hand in R code.   R code   is   information that   is   not asked for; see   above.
· For Part   B, you are allowed to   use   an AI tool   (such   as   ChatGTP),   but you   should   acknowledge   the   use of this and explain the way you   used   it.
· You can use the forum to raise   queries   during the   assessment,   but   only   if the   queries   concern
clarification of tasks   in the assessment. This option will only be available till 12 noon on March 17th, 2025.   From that time onward the forum will be   read-only till   March   19th.
Part   A 
Question   1 
For this question, you   have to download a data set that   is   identified   by   your   Student   ID   number.
· You can find the data   in the Section   ICA 2 on   Moodle. Your data   set   is   identified   by   your   student   ID   number.   Be careful to   identify your data specifically.   Marking   is   partly   based on student-specific
data analysis.
· If   your   ID   is   20001234 for   example, then   select   and   download   the   text   file      20001234.txt   and   put the file in the working directory of your R session.
· Read   in   the   file   in   your   R   session   by   the   command      dta   <- read.csv(file="20001234.txt") , and have a look at the data. Example of using R for this:
> dta <- read.csv(file="20001234.txt") 
> head(dta) 
y x 
1 8.27 1 
2 5.06 1 
3 12.14 1 
4 4.92 1 
5 6.30 1 
6 9.81 1 
· If you cannot   read   in the data   in   R, contact the   module   lead   as soon   as   possible   via   email:
[email   protected] .
· The data are created   in the format of a   100   × 2 table. The first   column   (   y )   is for   response   Y,   and the second column ( x ) identifies   the   level   of the treatment   variable.
Your data concern a one-way ANOVA experiment regarding the height   of a flower   plant.   Response   Y   is   the   response   in centimeters, and    x   identifies the five treatment   levels. Values    x   =   1,   2,   3,   and   4 correspond with the use of four different fertilisers. The value    x   = 5   corresponds with   the   no-fertiliser   treatment. The aim of the experiment   is to establish how   the   height   of the   plant   is   affected   by   choice         regarding fertilisers. 
For the statistical inference, use a   significance   level   of   5%.
(a) Consider the hypothetical case where data for this experiment   are   collected   by   someone   who   uses   her garden. Say she collected the data   by   using the front   and the   back   garden   as   follows:   plants with         fertiliser    x =   1 and    x = 2   in the front garden, and the   plants with   the   other   treatment   levels   in   the   back   garden.   Explain   briefly and   in simple terms (without using the word   “randomisation”) why   this   is   not   a good way to collect the   data. [3] 
(b) Potassium   is a common   ingredient   in fertilers. Consider the   hypothetical case that fertiliser      x =   1   has   twice the amount of potassium compared to fertilisers   identified   by      x = 2, 3,   and 4.   Would   this undermine your statistical inference?   Explain your answer. [3] 
(c) Define a one-way linear   ANOVA model for response Y with   an   intercept.   Define   the   model   such   that   the intercept can be estimated   by the   mean   of the   observed   values for   Y under   the   no-fertiliser treatment. Write down the model equation and specify this   equation   completely   for   your   data. [8] 
(d) Fit the   model   in (c) to your data and report   the ANOVA table with clearly   defined   rows   and   columns. Using the model definition in (c),   define   the   hypothesis for   testing   whether   all   five   treatment   group   means   are equal. Test this 代 写STAT0045 In-course Assessment 2 (2024/25 SR
代做程序编程语言  hypothesis using the ANOVA table.   Be explicit about the distribution you   use for   this            test. [4] 
(e) Provide the   point estimates for all the   model   parameters   in (c). [6] 
(f) Define the estimator of the   intercept   in the   model   in (c) as a function of response   mean(s)   and   derive   the variance of this estimator as a function of the error variance   σ   2      and the sample   sizes   for   the treatment levels. Clearly explain your derivations. [8]
Question 2 
(a) Show   how to   derive

in Section 2.6.3.4.   Do   not derive anything that   is already shown   in   the   lecture   notes;   solve   for   a using   the   equations that are available   in the   notes. Mind that a previous   version   of the   lecture   notes   contained   a typo   in the expression for a. [6] 
Consider stratified sampling with the following   specifications:
Stratum 
Stratum size 
Strata variance 
1 
2000 
4 
2 
5000 
4 
3 
3000 
16 
4 
3000 
16 
5 
2000 
64 
(b) Consider that the variance of the stratified sample mean   Y-ST      is fixed   at   1/10. Assume that   costs   are   defined   by  where c0    =   100, and   (c1,   c2,   c3,   c4,   c5   )   =   (1, 2, 1, 2,   4).   Derive the
optimal strata sample sizes nℓ , for ℓ   =   1, 2,   3,   4, 5.   Explain your derivation. Hint: you   may want to use   R for the computation,   but do   not   include   R code   in your answer. [14] 
Question   3 
Consider the following randomised response (RR) design for   a   yes-or-no question   that   asks respondents whether or not they have committed fraud.   Instead of answering   the   question   directly,   the   respondent throws a dice and keeps the outcome   of the throw   hidden   from   the   interviewer.
· If the outcome of the   throw   is   1 or 2, then the   respondent   answers   yes.
· If the outcome of the throw is 6,   then   the   respondent   answers   no.
· If the outcome of the throw   is 3, 4, or   5, then   respondent   answers   yes or   no in   line   with   whether   or not   he or she   committed   fraud.
Assume that   respondents follow the   RR design.   Let π   1    denote the   probability that a   respondent   has   committed fraud.
(a) For this   RR design, give the values of the conditional probabilities   P(observed yes|latent yes)   and P(observed no|latent no), where observed refers to the data collected,   and   latent refers   to   the unknown status   regarding fraud. [7] 
(b) The observed data are given   by 300 yes-answers,   and   500   no-answers.   Estimate   π   1    and   calculate   the standard error for this estimate.   Explain your answers. [8] 
Consider the   RR design by Warner as specified on Slide   109.   Define   Yi      =   1 when   respondent   i   used illegal drugs, and Yi    = 0 otherwise.   Say   there   are   two   non-overlapping   groups   of   respondents   in   the   RR   survey; Group A and Group B.   Consider the   logistic   regression   model

where   xi      = 0 when   respondent   i   belongs   to   Group   A,   and   xi      =   1 when   i   belongs   to   Group   B.   Using ˆ
the   RR design, assume that the probability of observing a yes-response   in   Group   A is   estimated   by λA   .
(c) Define an estimate   of β0 as a function of A   .   Explain your derivation. [10]
Question 4 
(a) Consider Theorem 2.3   in Chapter 2 of the lecture   notes.   Using   the   notation   in   Section   2.8.2   provide   the final details of the proof; that   is,   show   that

is indeed an unbiased estimator of Var(Y-CL).   Provide   the   details   of your derivation.   Do not explain   the   existing equations   in the   proof of Theorem 2.3   in the lecture notes,   but   be   clear which of the   equations you use   in your   derivation. [9] 
There are ten schools   in a particular area. As part   of an   investigation   into   teaching   standards,   an            inspection team proposes to visit three of the schools and   administer a   test   to   all   of the   14-year   old   students   in each school visited. The school sizes (in   hundreds   of   pupils)   are   as follows:
School Size 
1 
22 
2 
18 
3 
17 
4 
21 
5 
11 
6 
23 
7 
16 
8 
22 
9 
26 
10 
24 
(b) Three   pseudo-random   numbers, distributed   uniformly on   (0, 1)   ,   have   been obtained   using   R. They   are 0.821, 0.228 and 0.307.   Use these to select   a   PPS   sample   of three   schools,   explaining your procedure clearly. [8] 
(c) Suppose that schools 4, 7 and 2 were   selected   (note   that   these   are not necessarily   the   schools   that         would be chosen using the random   numbers   provided   above),   and   that   the   average   test   results   for   these   three schools were   14.5,   16.7 and   13.6   respectively.   Use   these data to estimate the   average test   result         across all ten schools.   Provide an estimated standard error for your estimate. [6] 
Part   B 
For this   part you are required to write a short   report   discussing   aspects   of data   ethics for   a   given   scenario.
The scenario:   In the   UK,   housing   benefit can   help you   pay your rent   if you are   unemployed or   on   a   low   income.   If you receive benefit, then you need to   report   a   change   of circumstances for   you   and   anyone         else   in your house.   Examples of housing   benefit fraud are   not   reporting all   income   or   not   reporting   a
change of income.
In a   large city   in the   UK, the   manager who deals with   housing   benefit   in the city wants   to   use   data   science to help   identity fraud.The   manager’s   idea   is to use data from past   receivers of   housing   benefit who were   investigated   for   fraud.   Assume that for these people individual information   is   available   on whether or   not   fraud   was      detected.
The   manager envisages using the data to define a   statistical   prediction   model   and   next   to   use   this   model   to   identify current receivers of housing benefit who   are   likely   to   commit fraud.
You are asked to lead this   project. The   main statistical   parts   of the   project   are:   collecting   relevant   data, data analysis, defining a   model that can be   used for   prediction,   and   using   the   model   to   make   a   prediction   for current receivers of   housing   benefit.
Assume that the chosen   prediction   model   is a logistic regression   model   for   a   binary   response   variable   with value   1 for fraud and value 0 otherwise.
Instructions and guidelines for the report:
· Write a report that discusses the scenario with a   focus   on   data   ethics.   Limit   the   scope   of data   ethics to the   material that   is discussed in   STAT0045.
· You should explicitly use the following terms   in the report   (and   reflect on   the   concepts   attached   to   these terms): “data subject”, “model subject”, “fairness”, and   “transparency”.
· You should discuss to some extent the   importance   of GDPR   in   this   project   and   give   at   least   one   concrete example of a measure that you would implement   to warrant   that   GDPR   guidelines   are      followed.   In the discussion of GDPR you should explicitly use the term   “personal   data”   in   the            report.
· Assume the reader knows the logistic   regression   model; do not discuss   standard   aspects;   for   example,   how the   model   is defined or how to estimate   model   parameters.
· Give the   report   a title.
· Type the   report   in a text editor and add the word   count   at the   end   of the   report.   Use font   size   12.
· Write the   report   in   paragraphs and complete sentences.   Using a few   bullet   points   is OK,   but   do not write the   report as   a   list of   bullet   points.
· Maximum word count for the report (including the   title)   is 700 words.   Report   longer   than   700   words will be   penalised.
· If you use an   AI tool (see   instructions), then   use   an   appendix   to   acknowledge   this   use.   This   appendix does not count towards the   maximum word   count.
· You can add literature references to the   report.   References   do   not   count   towards   the   maximum   word count.   No   need to add   references to the   STAT0045 course   material.
Hints:
· There   is   no specific   need to use AI tools for this report.   Mind the danger   of   using AI tools;   see   the   slides on   Use ofAI Tools   in Chapter   1.
· Although   it   is fine to   refer to   literature   beyond the course   material, there   is   no specific   need to do   so.
· The aim of this assignment is to see whether you   are   able to   critically   reflect   on   aspects   of data   ethics   in a practical scenario.   Do not just enumerate definitions   or aspects   of   data   ethics,   focus   instead on some of the aspects and explain why they   are   important   in this   scenario.
· You are   not asked to solve   potential   problems   in this scenario, or   provide   details   of specific
actions. The   report should focus on   potential   issues with respect to   data   ethics   -   not   knowing   how   the   issues can   be addressed   in detail   is   OK.
Marking criteria: adherence to the above instructions and   guidelines,   and   the   quality   of the   presentation   (readability, structure, language). [100] 



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
