---
layout: essay
type: essay
title: "The Playbook of AI"
# All dates must be YYYY-MM-DD format!
date: 2024-04-25
published: true
labels:
  - AI
  - Education
---

### I. Introduction
Artificial intelligence has been integrating itself into society within the recent years, and it has undeniably become a powerful tool at every level. Professionals, educators, students, and many more occupations have benefited from AI. Especially in the field of software engineering, AI has become a "coding assistant" of sorts for many people. Whether AI is being used to write code, check for errors and redundancies, or explain a concept, the potential for AI as an integral part of software engineering seems unlimited. ChatGPT, GitHub Copilot, and Google Gemini have all proved to be useful in creating efficient and interactive projects.

### II. Personal Experience with AI:
I have used AI in class this semester in the following areas:

  1. Experience WODs e.g. E18\
To experience and gain the necessary knowledge, I did not employ AI into the Experience WODs. These WODs are meant to provide the fundamentals of the specified area or skill, which means that to fully understand        them, I wanted to go through the content with minimal assistance. If I could not complete the WOD, there were enough resources supplied from the course as well as documentation to help me finish the task.
  
  2. In-class Practice WODs\
Similar to the experience WODs, I used the in-class practice WODs to develop problem solving skills while under time pressure. The in-class practice WODs didn't hold any weight in terms of grade, therefore I figured I could use them to purely practice my own skills and not rely on AI.
  
  3. In-class WODs\
For the actual in-class WODs, I felt well prepared due to the experience and practice WODs done prior to the real thing. This allowed for minimal use of AI, which made an appearance one time throughout the WODs. When I decided to employ AI, I used ChatGPT to assist me in WOD: Javascript 3, which involved a database of UH Manoa graduates with their respective degrees and several other metrics regarding them.\
There were two goals: find the average number of graduates that also had awards at the time of graduation; and find the number of graduates with PhDs who were Hawaiian. In order to accomplish this task, I used the Underscore.js library to filter the database, pluck objects with specific properties, and reduce large quantities of data to one value. However, at the time of this WOD, I was not that familiar with Underscore, and looking through the entire library of methods would've left me with limited time to write the actual code. This is when I used ChatGPT, which found the methods I needed to finish my code, massively cutting down the total amount of time I spent on the problem.

  4. Essays\
Most of the essays written throughout this course allowed for a creative and personal touch to turn technically heavy concepts into relatable and interesting readings. The use of AI to write entire essays would take away that human touch and leave it as a regurgitation of some Wikipedia article. Thus, I did not employ AI to write essays. Rather, I used ChatGPT to help with making sentences more fluid. This would sometimes prove useful, providing a response that fit better in the theme of the essay. Other times, ChatGPT would provide a block of words that sounded more mechanical than human, which I ended up leaving out. In essence, I used ChatGPT and AI in general minimally in my essays since they would provide unengaging writing.

  5. Final project\
In the final project, I found that the use of AI actually hindered my progress. The project involved a lot of files that interacted with each other, with pages and components reading off of others. This proved to be difficult to pass on to ChatGPT in most cases, as I would have to pass multiple files of code into the AI, on top of figuring out what exactly to ask. For the most part, it seemed easier to look into the code and the web dev console rather than cycling code into ChatGPT. 
 
  6. Learning a concept / tutorial\
When it came to learning a concept or finding some tutorial for a skill, I found it more beneficial to look up the documentation or watch Youtube videos for information. Tutorialspoint, GeeksforGeeks, and StackOverflow have been a reliable source of information for a long time. I also can find more precise answers to questions and concepts when I use sources other than AI. I have found that AI typically gives a broad and general overview of concepts since the response it gives is based on what it is prompted on. If I know the bare minimum about a concept, I wouldn't be able to provide a question or prompt that would yield useful answers from ChatGPT. However, a basic question on a Google or Youtube search can lead to extensive research, which I find to be more fulfilling.
  
  7. Answering a question in class or in Discord\
Similar to learning a concept, I didn't employ AI much when searching for answers to questions posed in class or Discord. A normal Google search proved to be more than sufficient in providing answers. On top of that, since questions were open to the entire class, it was easy to seek solutions from peers who have encountered similar issues or had similar questions.
  
  8. Asking or answering a smart-question\
Building off of what was said above, having peers who share similar experiences creates an easy-access resource to answers. I didn't involve myself much on the Discord when it came to asking and answering questions, however I did find myself going to those in my class as well as the professors and teaching assistants instead of AI when I needed assistance.
  
  9. Coding example e.g. “give an example of using Underscore .pluck”\
A solid example of my use of AI (ChatGPT specifically) is the same example from the WOD topic discussed above.
```
let testData = _.first(uhdata, 5);

//console.log(testData);

function averageDegrees(data) {
    let numAwards = _.pluck(data, 'AWARDS');
  let totalAwards = _.reduce(numAwards, function(memo,num) {
      return memo + num;});
    let denom = uhdata.length;
    return totalAwards / denom;
}

console.log(averageDegrees(uhdata));

function hawaiianPhDs(data) {
    let isHawaiian = _.filter(data, function(fieldname) {
      return fieldname["HAWAIIAN_LEGACY"] === "HAWAIIAN"; })
  let isDoctor = _.filter(isHawaiian, function(fieldname) {
      return fieldname["OUTCOME"] === "Doctoral Degrees";
  })
  let doctorAwards = _.pluck(isDoctor, 'AWARDS');
  let totalDoctor = _.reduce(doctorAwards, function(memo, num){
      return memo + num;
  })
  return totalDoctor;
}

console.log(hawaiianPhDs(uhdata));
```
In this code, I used ChatGPT to look through the Underscore library to find the following methods: .pluck(), .filter(), and .reduce(). With these methods, I was able to write two functions that operated on the given UH Manoa dataset.

  10. Explaining code\
The code I have written, seen, and read within the scope of this course has been realtively simple and easy to understand. The code became a bit harder to understand once we started to implement applications using Meteor and MongoDB, however with some time and effort to read through and test the code I was able to understand what was going on. For this specific topic, I didn't feel the need to use ChatGPT. However, outside of the scope of the course, I have used ChatGPT to explain code, specifically code realting to data structures and algorithms. This has provided useful explanation as to what is happening, but that is beside this course.
  
  11. Writing code\
As it was mentioned before, I have used ChatGPT to find methods to implement in my code, but I haven't used it to write entire code blocks in this course. Similarly to the above statements, outside of the scope of the course, I have used ChatGPT to write algorithms, and the code provided has proved to be efficient and accurately answers the problem statements I have prompted it. 
  
  12. Documenting code\
As for documenting code, I haven't found the need to use AI to document code. Whether it's documenting the download, installation, and setup, or leaving comments and summaries about the code and its scalability, I've found that writing my own documentation would be sufficient. AI could potentially cause problems with documentation as well, since it could misinterpret the code. 
  
  13. Quality assurance \
Within the scope of this course, I haven't relied on AI to find errors in my code. Most of the errors and the quality of my code can be fixed through inspecting the terminal for ESLint errors or the web dev tool on Google when applications start to break. Through the use of those tools, I've been able to determine and solve the problems that I have encountered. As before, I have used ChatGPT to fix other code outside of this course, mainly for finding issues regarding segmentation faults.
  
  14. Other uses in ICS 314 not listed above\
Other than the uses listed above, I can't think of other uses that I could use AI for within the scope of this course.

### III. Impact on Learning and Understanding:
AI is a powerful tool that can be utilized for both educational and professional purposes. 

### IV. Practical Applications:


### V. Challenges and Opportunities:


### VI. Comparative Analysis:


### VII. Future Considerations:


### VIII. Conclusion:
