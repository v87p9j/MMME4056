java cESSENTIAL INFORMATION
MODULE CODE MODULE TITLE ASSESSMENT TYPE
MMME4056 Integrated Systems 
Analysis
Simulink and Report
COURSEWORK TITLE WEIGHT (INDICATIVE EFFORT)
MMME4056, ISA 2024, COURSEWORK 30% (Approx. 10-15
hrs)
SUBMISSION DATE SUBMISSION TIME SUBMISSION METHOD
15/11/2024 15:00 Moodle
FEEDBACK DETAILS
Feedback will be provided within 20 working days and will consist of an individual feedback 
form. Please note the marks released on Moodle are raw. If you have made a late submission 
and it is not covered by an EC or an accommodation then the deductions will be made when I 
submit the marks to the board after the exams. 
LEARNING OUTCOMES ASSESSED (IN BOLD)
1. Demonstrate an understanding of the concept of system behaviour and the design of 
experiments for characterising system components. - AHEP4: 2, 6 
2. Critically evaluate and analyse complex dynamic systems behaviour using an 
appropriate numerical or analytical methodology - AHEP4: 1, 2, 3, 6 
3. Evaluate the reliability of the separable system components, coupled system 
components and systems as a whole - AHEP4: 6, 9
SUBMISSION REQUIREMENTS
• This exercise constitutes 30% of the total course mark and is marked out of 100. 
Marks for individual sections are indicated for that section.
• Submit your coursework via MOODLE as a ZIP file. This ZIP-file should contain the 
coursework report itself (as a pdf document) and all files that you used in the CW. 
Please adopt the file-naming suggested in this coursework specification. More details 
about ‘WHAT TO SUBMIT’ can be found in the ASSESSMENT DETAILS.
• It must be possible to open the SIMULINK models submitted using MATLAB release 
R2023 or later. Models presented in different releases that cannot be opened will not
be marked. 
• Your report should not exceed 20 pages including the cover page, references, and 
appendixes.
• Your Coursework should have a front page which will have your name and student 
number.
• Text elements should be typed. Ideally in Arial 11 point.
• Drawings and figures must be made by computer. Drawings and figures may not be 
copied from the internet. In ALL cases they should be appropriately titled and 
captioned. The titles and captions should be clear and legible. 
• You may not discuss the details of your answers with other students. Software checks 
will be made to ensure no copying or plagiarism has occurred.
• Whenever you talk about someone else’s work (including journal papers, books, 
conference papers, technical reports, theses/dissertations, websites, etc.) if necessary,
you must include a reference to the original source of this information. You should use 
the IEEE referencing style for your report. 
MMME4056... Integrated Systems Analysis
COURSEWORK 
SYSTEM DESCRIPTION.
Figure 1 shows a floating wind turbine of spar-buoy type. These floating 
supports for wind turbines achieve stability by having a centre of mass 
below the centre of buoyancy (i.e. the centre of gravity of the displaced 
water).
Spar-buoy floating arrangements are considered by some to be suitable for 
very deep water. They are relatively compliant in “pitch”. That is to say, 
when the wind blows and exerts a downwind thrust force on the rotor of 
the wind turbine, the entire structure rocks backwards a little bit. As the 
structure is moving backwards relative to the oncoming wind, the relative 
wind speed reduces and so a coupling arises between the thrust force, F(t), 
acting on the turbine and the angle of tilt, (t), of the platform. This 
coursework is based on modelling the dynamics of such a floating wind 
turbine platform and applying the methods taught within MMME4056.
The downwind thrust on a wind turbine rotor is not a simple function of 
the wind speed, v(t). Every modern wind turbine has a particular fixed 
rated wind speed vrated. For wind speeds lower than the rated wind speed 
(v(t)  vrated), 
the turbine is not able to absorb all of the power available and the 
controller must deliberately spill some power by pitching the blades 
suitably. This results in a different downwind force relationship …
𝐹(𝑡) = 𝑎 × 𝑣𝑟𝑎𝑡𝑒𝑑
3⁄𝑣(𝑡). Figure 2 below shows a typical relationship 
between wind speed and the downwind thrust force acting on a wind turbine. 

q
Fig. 1: A Spar-buoy floating 
 wind turbine support
F
H
Fig. 2: Downwind thrust vs. (relative) wind speed.
vrated
Vcut-out
Wind speed, v →
Downwind thrust, F
→
OVERALL REQUIREMENTS
The requirement of this coursework is to understand this floating wind turbine as a simple dynamic system, to 
simulate its behaviour as wind-speed changes using SIMULINK and to analyse its behaviour at two different 
equilibrium states using methods taught in the course. 
The submission should be based on what is explicitly asked for in this coursework specification. The primary 
material being marked is a report – although you are asked to submit your SIMULINK models also. It must be 
possible to open the SIMULINK models submitted using the version of MATLAB presently installed on 
University computers. Models prepared in more modern releases will not be marked. 
There are no additional marks for long reports!
FILES PROVIDED TO YOU – AND WHAT THEY DO.
CW_Spec.docx : This file. It contains the coursework specification.
f_diesel.m : A MATLAB function n代 写MMME4056、MATLAB
代做程序编程语言ot directly related to this coursework but supplied to help illustrate 
how a SIMULINK model can call a MATLAB function.
f_thrust.m : An MATLAB function that is not complete. You should complete this function by 
modifying each line of code carrying the comment % Modify this line
In some cases, the modification simply involves you inserting the appropriate 
numerical values. In the remaining cases, you should insert the correct formula.
sim_diesel.slx : A SIMULINK model calling the function f_diesel.m. 
As well as showing how to call an Interpreted MATLAB Function in SIMULINK,
this also shows how to transfer data into the MATLAB workspace so that you can 
obtain plots using MATLAB directly.
stud_data.xls : An EXCEL spreadsheet containing one unique row of data for each student. 
Each row contains (in this order) … {vrated, a, J, k, c, H, p, q…}
start_here.m : A MATLAB script. This opens up a SIMULINK model of the diesel engine only, 
() and then runs the model and plots both  and  vs. time. You might
choose to copy and then modify this so as to use it as a way to open and run your own
SIMULINK model. You can run  either by clicking the big green 
arrowhead in the top toolbar of the editor or else by just typing >>start_here 
at the MATLAB command prompt).
WHAT TO SUBMIT
Submit your coursework via MOODLE as a ZIP file. This ZIP-file should contain the coursework report itself (as a 
WORD or PDF document) and all files that you used in the CW. 
IMPORTANT: Please make clear on the first page of the report which student you are by identifying which 
Student ID# (SID# in the spreadsheet) applies to you (a number less than 401). If, for some reason, you do not find 
your name in the spreadsheet, please contact the academic in charge of this coursework to get one. For the 
purposes of your report, please refer to this number as the “SID_No”. (Student Identification number) on your 
report clearly.
 Marks will be deducted if you do not show this information clearly on page 1.
The coursework report should comprise:
• A response to Task 1 (the Table and, at most, 2 further sentences)
• A response to Task 2 (the corrected function, , and four numerical answers)
• A response to Task 3 (maximum 2 pages). This should include an explanation of how you 
applied an algebraic or iterative approach to finding the two equilibrium conditions and a 
description of each equilibrium condition comprising {𝐹9.5,𝜙9.5, 𝑞9.5} and {𝐹14,𝜙14, 𝑞14}. 
• A response to Task 4 which should comprise
- a legible view of the SIMULINK model (on a single page)
- an explanation in text of how you have applied the initial conditions
- the plot of q(t) vs. t.
• A response to Task 5 (1 page) comprising the SIMULINK Model and a plot of q(t) vs. t.
• A response to Task 6 ( 𝑣𝑐𝑢𝑡𝑜𝑢𝑡, 𝐹(𝑡) = (𝑎 × 𝑣𝑟𝑎𝑡𝑒𝑑
3⁄𝑣𝑐𝑢𝑡𝑜𝑢𝑡) ∗ exp (−5(𝑤(𝑡) − 𝑣𝑐𝑢𝑡𝑜𝑢𝑡))
Otherwise if 𝑤(𝑡) ≥ 𝑣𝑟𝑎𝑡𝑒𝑑, 𝐹(𝑡) = 𝑎 × 𝑣𝑟𝑎𝑡𝑒𝑑
3⁄𝑤(𝑡)
Otherwise 𝑤(𝑡)  and present that 
function in your report. Then call that function directly from the MATLAB for four different wind speeds: 
{ 3m/s, 9.5m/s, 14m/s, 28m/s }. Report the results. 
HINT: To get the answer for 9.5m/s, type … f_thrust( 9.5) at the MATLAB command prompt. 
[10 marks]
Task 3. Without using SIMULINK, determine an equilibrium condition for the dynamic system at the wind 
speeds 9.5m/s and 14m/s. For each of these speeds, report the following steady values, 
𝐹9.5 = , 𝐹14 = 
𝜙9.5 = , 𝜙14 = 
𝑞9.5 = , 𝑞14 = 
HINT: There is no “closed-form” solution here so you will have to apply an iterative approach of some sort. A 
manual iteration process is fine. You do not have to write any code to implement an iterative solution automatically 
or to use any built-in iterative methods within MATLAB. 
[15 marks]
Task 4. Now create a SIMULINK model of the system and run this model over a period of 500s with a constant 
wind-speed of 9.5m/s taking the initial conditions to be (0) = 0.15 rad and 𝜙(0) = 0. Plot q(t) vs. t . 
[25 marks]
Task 5. Modify the SIMULINK model from Task 4 so that the wind speed is now varying sinusoidally 
according to 𝑣(𝑡) = 9.5 + 0.2𝑐𝑜𝑠(0.2𝑡). Change the initial conditions so that (0) =  determined from Task 3. 
Plot q(t) vs. t over 500s.
[10 marks]
Task 6. Create state-space representations of the system for each of the two different equilibrium conditions 
discovered in Task 3. In each case, treat v(t) as the only input and q(t) as the only output and report the matrices, 
{A, B, C, D} for both cases separately. For the case of v(t)  9.5 m/s, use these matrices to develop an alternative 
prediction for q(t) vs. t from Task 5. Create a plot containing two curves on the same graph representing q(t) vs. t. 
One of those curves should use the data from Task 5 and the second curve should use the data from Task 6.
[15 marks]
Task 7. Calculate the eigenvalues of the matrix A for the case v(t)  14 m/s and interpret what these 
eigenvalues tell you. Modify the SIMULINK model from Task 4 so that the input wind speed is now a steady 
14m/s. Set the initial conditions to be (0) = ( + ) and run this model for 500s. Once again, plot q(t) vs. t. 
Comment on any connections between what you see from the SIMULINK model output and what you found from 
the eigenvalues of matrix A. 
[15 marks]

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
