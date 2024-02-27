---
comments: True
layout: notebook
title: Trimester 2 Individual Review
description: This is the individual review to showcase my feature that follows collegeboard guidelines for trimester 2.
type: ccc
author: Prakruti Bhatt
toc: True
courses: {'csp': {'week': 20}}
---

# **Trimester 2 Individual Review**

#### N@TM Project Overview:
Me and my team for this Night at the Museum project (Vidha, Isabelle, Hannah), had the wonderful opportunity to make a mood tracker! We implemented numerous features that helped track a user’s mood, release any pent up stress, and motivate users! 

#### The Feature I Worked On:
The feature that I worked on was a quote repository. We often find quotes that we find inspiring and motivational and I wanted to make something to store that information for reference if anyone wanted to look back at those life-changing quotes. The feature lets you input the quote, quote author, and your opinion on that quote. This information is documented/regulated through the backend repository and saved quotes can be viewed in a quote archive. 

# Component A: Programmed Feature/CPT Requirements

| College Board Requirements  | My work  |
|----------|----------|
| Instructions for input from one of the following: the user, a device, an online data stream, a file |![Alt text](/pb2csp/images/blog1.png) - The code above uses HTML input fields and a textarea to take input from the user. The user can enter a motivational quote, the quote author, and their opinion on the quote. |
| Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the user's purpose. |![Alt text](/pb2csp/images/blog2.png)- The quoteObject is structured as an object, which can be considered a form of collection. The Fetch API sends the quoteObject (data collection) to the server for storage, demonstrating the use of data collection for program functionality. |
| At least one procedure that contributed to the program’s intended purpose where you have defined: the name, return type, one or more parameters. |![Alt text](/pb2csp/images/blog3.png)-The submitQuote function is a procedure that contributes to the program's purpose by handling the submission of a quote. It has no return type. No explicit parameters are defined in the function signature. The function relies on accessing the values of the HTML elements with IDs: 'quote', 'quote-author', and 'opinion' to gather user input.|
| An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure	| ![Alt text](/pb2csp/images/blog4.png) -Here, the code constructs a quoteObject by gathering data from the input fields (quote, quoteAuthor, and opinion). This is a sequential process where the data is organized into an object for further use. ![Alt text](/pb2csp/images/blog5.png)- Before submitting the quote, the code checks if any of the required fields (quote, quoteAuthor, opinion) are empty. This is a selection mechanism that ensures all fields are filled before proceeding with the submission. If any field is empty, it triggers an alert asking the user to fill in all fields. The image below (using fetch function to call to the backend) uses the Fetch API to make an asynchronous HTTP request to the server. It sends the quoteObject to the server for storage. This is Iteration using Fetch API (Asynchronous Iteration). |
| Calls to your student-developed procedure|![Alt text](/pb2csp/images/blog6.png)- This part of the code represents the call to my backend for submitting a quote. The submitQuote function uses the Fetch API to send the quoteObject to the server. |
| Instructions for output (tactile, audible, visual, or ) based on input and program functionality | ![Alt text](/pb2csp/images/blog7.png) - This part of the code employs a conditional structure where, if the server response is successful (.then), an alert displays the received message; otherwise (.catch), an error message is alerted, ensuring appropriate user feedback based on the server. Provides visual output in the form of alerts, notifying the user whether the quote submission was successful or if an error occurred. |

# Component B: Video
<a href="https://drive.google.com/file/d/19kuanAAeSlkN07fHxQ5Xv6tLIF8bXCJp/view?usp=sharing" class="button" style="padding: 10px; background-color: #800000; color: #fff; text-decoration: none; border-radius: 5px;">Click here to view the video</a>

| Collegeboard Requirements | My Video |
|----------|----------|
| Input to program | This is highlighted in the video when we click on the quote repository feature and enter the information. This information (the quote, quote author, and quote opinion) is entered accordingly at the beginning of the video. |
| At least one aspect of the functionality of your program | There is a quote storage where you can view the quotes that you wrote up and look back on some influential quotes and the opinions that you had on them. This showcase is demonstrated in the video.|
| Output produced by program | Once input is entered and submitted, there is an output/popup which lets you know if the quote has been submitted successfully or not. When you redirect to the quote showcase, the input, if successfully entered, will be saved as a result that you can refer back to. |
| My video does not have: | The video does not display any other feature or its code and does not include a background voice narration. |
| My video is: | Exactly 1 minute long in the form of a .mp4 file and 5.60 GB. |





