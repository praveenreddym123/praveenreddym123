
<!DOCTYPE html>
<html>
<head>

<!-- Remove the Comments and fill up the relevant code -->

<style type="text/css">

body{
/* Fill the attribute */background-color: #FFAACC;
}

h1
{
color:#770080;

font-family: Courier New;
font-style:italic;

text-align: center;

}
table
{
    text-align: justify;
}
form
{
    
margin :0 auto;
width:300px;
}

#result
{
/* Fill the attribute */color:#770080;

/* Fill the attribute */font-weight:bold;

}
</style>

<title>Infotech College</title>
<script>
function calculateFeedbackRating()
{
   
   /* Fill  the code  for Javascript function */
   var feed=document.getElementById("trainerFeedback").value;
  
   var trainerName=document.getElementById("trainerName").value;
   var feedbackRate;
   
   if(feed=="Excellent")
   {
       feedbackRate=5;
   }else if(feed=="Very Good")
   {
       feedbackRate=4;
   }
   else if(feed=="Good")
   {
       feedbackRate=3;
   }else if(feed=="Average")
   {
       feedbackRate=2;
   }else
   {
       feedbackRate=1;
   }
  
   document.getElementById("result").innerHTML="Feedback rating of "+trainerName+" is "+feedbackRate;
   return false;
}

</script>

</head>
<body onsubmit="return calculateFeedbackRating();">
<!--Write necessary code wherever needed to complete this knock out code challenge  -->
<h1>College Training Feedback Form<!-- Fill the text --></h1>
<form>
<table >

<tr>
<td>Participant Name<!-- Fill the label for participant name--></td>
<td><input type="text" name="participantName" id="participantName" placeholder="Enter your name" required><!-- Fill the code for participant name--></td>

<tr>
<td>College Name<!-- Fill the label for college name--></td>
<td><input type="text" id="collegeName" name="collegeName" required><!-- Fill the code for college name--></td>
</tr>

<tr>
<td>Participant address<!-- Fill the label for participant address--></td>
<td><textarea name="participantAddress" id="participantAddress" rows="5" cols="20" required></textarea><!-- Fill the code for participant address--></td>
</tr>

<tr>
<td>Gender<!-- Fill the label for gender--></td>
<td><input type="radio" id="gender1" name="gender" value="Male" required>Male
<input type="radio" id="gender2" name="gender" value="Female" required>Female
</td>
</tr>

<tr>
<td>Email ID<!-- Fill the label for email--></td>
<td><!-- Fill the code for email -->
<input type="email" id="email" name="email" required></td>
</tr>



<tr>
<td>Mobile Number<!--Fill the label for mobile number--></td>
<td><input type="text" id="mobileNumber" name="mobileNumber"  pattern="[789]{1}[0-9]{9}" required ><!-- Fill the code for mobile number --></td>
</tr>

<tr>
<td>Trainer's Name<!--Fill the label for trainer name--></td>
<td><input type="text" name="trainerName" id="trainerName" required ><!-- Fill the code for trainer name --></td>
</tr>

<tr>
<td>Course Name<!--Fill the label for course name--></td>
<td><input type="text" id="courseName" name="courseName" required><!-- Fill the code for course name --></td>
</tr>

<tr>
<td>Course Completion date<!--Fill the label for date of completion--></td>
<td><input type="date" id="dateofcompletion" name="dateofcompletion" required><!-- Fill the code for date of completion --></td>
</tr>

<tr>
<td>Trainer's Feedback</td>
<td><input type="text" name="trainerFeedback" id="trainerFeedback" list="feedback" autocomplete="on" required>
		<datalist id="feedback" autocomplete="on">   
  		<option value="Excellent">Excellent
		<option value="Very Good">Very Good
		<option value="Good">Good
		<option value="Average">Average
		<option value="Below Average">Below Average
		</datalist>

</td>
</tr>


<tr>
<td><input type="submit" id="submit" value="Submit Feedback" name="submit" > <!--Fill the code for submit button--></td>
<td><!--Fill the code for reset button-->
<input type="reset" id="reset" name="reset" value="Clear"> </td>
</tr>

<tr>
<td colspan="2">
<!--Fill the code for div tag-->
<div id="result"></div>
</td>
</tr>

</table>
</form>
</body>
</html>
