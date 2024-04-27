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
To experience and gain the necessary knowledge, I did not employ AI into the Experience WODs. These WODs are meant to provide the fundamentals of the specified area or skill, which means that to fully understand        them, I wanted to go through the content with minimal assistance. If I could not complete the WOD, there were enough resources supplied from the course to help me finish the task.
  2. In-class Practice WODs\
Similar to the experience WODs, I used the in-class practice WODs to develop problem solving skills while under time pressure. The in-class practice WODs didn't hold any weight in terms of grade, therefore I figured I could use them to purely practice my own skills and not rely on AI.
  3. In-class WODs\
For the actual in-class WODs, I felt well prepared due to the experience and practice WODs done prior to the real thing. This allowed for minimal use of AI, which made an appearance one time throughout the WODs. When I decided to employ AI, I used ChatGPT to assist me in WOD: Javascript 3, which involved a database of UH Manoa graduates with their respective degrees and several other metrics regarding them.\
There were two goals: find the average number of graduates that also had awards at the time of graduation; and find the number of graduates with PhDs who were Hawaiian. In order to accomplish this task, I used the Underscore.js library to filter the database, pluck objects with specific properties, and reduce large quantities of data to one value. However, at the time of this WOD, I was not that familiar with Underscore, and looking through the entire library of methods would've left me with limited time to write the actual code. This is when I used ChatGPT, which found the methods I needed to finish my code, massively cutting down the total amount of time I spent on the problem.
The code I was able to produce is below:
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
  5. Essays
Most of the essays written throughout this course allowed for a creative and personal touch to turn technically heavy concepts into relatable and interesting readings. The use of AI to write entire essays would take away that human touch and leave it as a regurgitation of some Wikipedia article. Thus, I did not employ AI to write essays. Rather, I used ChatGPT to help with making sentences more fluid. This would sometimes prove useful, providing a response that fit better in the theme of the essay. Other times, ChatGPT would provide a block of words that sounded more mechanical than human, which I ended up leaving out. In essence, I used ChatGPT and AI in general minimally in my essays since they would provide unengaging writing.

  6. Final project\

  7. Learning a concept / tutorial\

  8. Answering a question in class or in Discord\

  9. Asking or answering a smart-question\

  10. Coding example e.g. “give an example of using Underscore .pluck”\

  11. Explaining code\

  12. Writing code\

  13. Documenting code\

  14. Quality assurance \

  15. Other uses in ICS 314 not listed above\


### III. Impact on Learning and Understanding:


### IV. Practical Applications:


### V. Challenges and Opportunities:


### VI. Comparative Analysis:


### VII. Future Considerations:


### VIII. Conclusion:
