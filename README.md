# CalculateLetterGrade
Calculate Letter Grade
Extra 2-1	Design a simple form
In this exercise, you’ll design a form that lets the user enter a number grade and then displays the letter grade when the user clicks the Calculate button. 
 
1.	Start a new project named CalculateLetterGrade in the Extra Exercises\Chapter 02\CalculateLetterGrade directory. Be sure to store the solution in its own directory.
2.	Add the labels, text boxes, and buttons to the form as shown above. Then, set the properties of these controls as follows:
Default name	Property	Setting
label1	Text	&Number grade:
TextAlign	MiddleLeft
TabIndex	0
label2	Text	Letter grade:
TextAlign	MiddleLeft
textBox1	Name	txtNumberGrade
TabIndex	1
textBox2	Name	txtLetterGrade
ReadOnly	True
TabStop	False
button1	Name	btnCalculate 
Text	&Calculate
TabIndex	2
button2	Name	btnExit
Text	E&xit
TabIndex	3
3.	Now, set the properties of the form as follows:
Default name	Property	Setting
Form1	Text	Calculate Letter Grade
AcceptButton	btnCalculate
CancelButton	btnExit
StartPosition	CenterScreen
4.	Use the Form Designer to adjust the size and position of the controls and the size of the form so they look as shown above.
5.	Rename the form to frmCalculateGrade. When you’re asked if you want to modify any references to the form, click the Yes button.
6.	Save the project and all of its files.
Extra 3-1	Code and test the Calculate Letter Grade form
In this exercise, you’ll add code to the Calculate Letter Grade form that you designed in extra exercise 2-1. Then, you’ll build and test the project to be sure it works correctly.
1.	Open the CalculateLetterGrade project in the Extra Exercises\Chapter 03\CalculateLetterGrade directory.
2.	Display the form in the Form Designer, and double-click the Calculate button to generate a Click event handler for it. Then, add this statement to the event handler to get the number grade the user enters:
decimal numberGrade = Convert.ToDecimal(txtNumberGrade.Text);
3.	Add this statement to the event handler to declare and initialize the variable that will hold the letter grade:
string letterGrade = "";
Then, add this if-else statement to set the letter grade:
if (numberGrade >= 88)
{
    letterGrade = "A";
}
else if (numberGrade >= 80 && numberGrade <= 87)
{
    letterGrade = "B";
}
else if (numberGrade >= 68 && numberGrade <= 79)
{
    letterGrade = "C";
}
else if (numberGrade >= 60 && numberGrade <= 67)
{
    letterGrade = "D";
}
else
{
    letterGrade = "F";
}
4.	Add this statement to display the letter grade in the Letter Grade text box:
txtLetterGrade.Text = letterGrade;
5.	Finally, add this statement to move the focus back to the Number Grade text box:
txtNumberGrade.Focus();
6.	Return to the Form Designer, and then double-click the Exit button to generate a Click event handler for it. Then, add this statement to the event handler to close the form:
this.Close();
7.	Run the application, enter a number between 0 and 100, and then click the Calculate button. A letter grade should be displayed and the focus should return to the Number Grade text box. Next, enter a different number and press the enter key to display the letter grade for that number. When you’re done, press the Esc key to end the application.

 Email me if you have any qeustions 
# SegvanJohnson@gmail.com
