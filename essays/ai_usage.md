---
layout: essay
type: essay
title: "AI usage in Software Engineering"
# All dates must be YYYY-MM-DD format!
date: 2024-12-17
published: true
labels:
  - ICS 314
  - AI Usage
  - ChatGPT
  - Co-Pilot
---
<div>
  <img src="https://blog.logomyway.com/wp-content/uploads/2023/08/open-ai-chatgpt.png" width="40%">
</div>

## Introduction

With how prominent AI is in school today, it is impossible to stray away from it. In my ICS 314 class, I chose to use it primarily for quality assurance purposes such as asking it to debug code for me when I encounter errors, or using it to help me explain and walk me through code. Using AI helped me further understand the software engineering topics we went over and helped me keep up with this very fast paced course.

## Personal Experience with AI

1. **Experience WODs**
<br>
AI was very useful for the experience WODs such as E18, when working with big datasets, manipulating them with typescript was challenging to understand at first, however for these WODs ChatGPT was very helpful and knew exactly what to do almost every single time.

2. **In-class Practice WODs**
<br>
For the in-class practice WODs, I was a little more reliant on AI usage since the practice WODs provided me with time to prepare for the real WOD and understand it prior to taking the actual WOD. For example, on the React WOD, I was having trouble making a nice background image, I used ChatGPT to help me find a workaround and implemented it myself during the in-class WOD.

3. **In-class WODs**
<br>
While doing the in-class WODs, I chose to only use AI if I was stuck or confused on what to do. I also refrained from using it on the later WODs such as the React, Next.js and HTML WODs. I noticed that its usefulness gradually decreased as the WODs went on since AI’s such as ChatGPT struggle with completely understanding what the instructions want us to do.

4. **Essays**
<br>
I did not want to use ChatGPT to write any of the essays as they are meant to showcase my writing skills to the world. With that being said, I do choose to use it strictly for grammar or punctuation purposes and for ideas to write about if I’m running out of them.

5. **Final Project**
<br>
I used AI’s such as Co-Pilot and ChatGPT for the final project since the final project required me to implement a lot of things that I had no idea how to implement. A good example of this is when I wanted to include a way to export a table as an excel file. ChatGPT helped me understand this concept and told me what to download to implement it to my project.

6. **Learning a concept / tutorial**
<br>
Personally, I prefer to learn through videos and in person classes. I chose to use YouTube as a resource to teach me a concept rather than ChatGPT to accommodate my learning preferences.

7. **Answering a question in class or in Discord**
<br>
For answering a question in class, ChatGPT proved to be beneficial due to us covering a lot of unknown topics at the time. It helped us provide valuable input to the class discussion prior to our lectures.

8. **Asking or answering a smart-question**
<br>
In regards to answering smart-questions, ChatGPT was also very useful because asking smart questions to ChatGPT helps it provide a better response to your question. For example asking ChatGPT a detailed question such as 

9. **Coding example**
<br>
An example of a problem I used ChatGPT to solve is when I was doing my final project, I encountered a problem with deleting users from the database. The problem was due to the User model having relations to other models that also had to be deleted. ChatGPT recommended me to use onDelete: Cascade, to also delete all relations.
```
model User {
  id                   Int         @id @default(autoincrement())
  email                String      @unique
  password             String
  role                 Role        @default(USER)
  firstName            String      @default("John")
  lastName             String      @default("Doe")
  approvedHours        Float       @default(0)
  pendingHours         Float       @default(0)
  phone                String?
  events               UserEvent[] @relation(onDelete: Cascade) // Delete associated events logs
  hoursLogs            HoursLog[]  @relation(onDelete: Cascade) // Delete associated hours logs
  createdAt            DateTime    @default(now())
  updatedAt            DateTime    @updatedAt
  status               String      @default("pending")
}
```
10. **Explaining code**
<br>
ChatGPT is very helpful when it comes to explaining what your code does. It helped me greatly with the final project when I needed to read and understand the code that my peers made so that I could apply my changes.

11. **Writing code**
<br>
For code writing ChatGPT helped me greatly when it came to implementing all the various topics we learned throughout the semester. Learning a new concept week to week can be a bit overwhelming. Thankfully with ChatGPT, I could understand the topic and see how it’s used properly.

12.	**Documenting Code**
<br>
I did not deliberately use ChatGPT to document my code, however changes to your code that ChatGPT makes are automatically commented in your code making it easier to see what ChatGPT added. It did prove useful however I did not use it for documentation purposes.

13.	**Quality assurance**
<br>
Quality assurance has got to be the most useful thing that ChatGPT provides. Asking ChatGPT to debug your code, and having it provide you with multiple ways to solve your problems helps save a lot of time coding. Usually I format my questions by asking the question, providing my code, and then giving ChatGPT the error message so it can diagnose my problem specifically.

14.	**Other uses in ICS 314 not listed**
<br>
N/A, all uses have been covered above.

## Impact on Learning and Understanding

Incorporating AI to my learning of software engineering has proved extremely beneficial overall. It helped deepen my knowledge on software engineering topics and also enhance my problem solving abilities. Using ChatGPT once to solve a problem helps me understand the thought process that went into solving it and allows me to apply it myself and deepen my understanding of the topic.

## Practical Applications

I have used AI for my real-world final project. My final project actually had me working with a client with the Sail Kokokahi sailing club. AI was very helpful for making a project that fulfilled all of the clients needs since they changed a bit with every email I sent him. AI is very proficient at addressing real-world software engineering challenges, you just have to send ChatGPT all of your code and clearly state what you need to ensure it understands what you want to accomplish.

## Challenges and Opportunities

I noticed that when working with projects that contained multiple files, ChatGPT understandably had a difficult time understanding how to solve your problem. I tried to use Co-Pilot instead since it is integrated to VSCode and I thought that it would be able to accurately solve the problem since it has access to all of the code in the project, however Co-Pilot was not very useful beyond finishing a few lines of code.

## Comparative Analysis

Personally, I prefer traditional teaching methods to AI-enhanced approaches. When it comes to understanding the topic on a deeper level AI is great, but for actually learning the topic, I prefer to be in a classroom setting. Taking notes on lectures and seeing a professional walk you step by step through a problem has always been my favorite aspect of learning. When it comes to retaining information, going over things in class is also better since you can practice it in-class to prepare you for your assignments.

## Future Considerations

I believe AI will continue to grow and develop. We have seen a plethora of new AI’s this year and they all are good at different things. It will continue to be a tool that software engineers have to master since it really is one of the best learning tools out there, and using and creating AI’s is  something that I myself would like to specialize in doing.

## Conclusion

Overall, using AI has helped me do very well in this class. Without it I would have had to spend even more time understanding the topics the course went over to achieve a similar level of success. It is a great tool to enhance learning at the college level, and I hope to see it continue to grow and improve in the future. In regard to using it in the course, I am grateful that this course is so understanding of the use of AI and I hope it continues to be AI friendly for years to come.
