---
title: Data Structures and Algortihms Learning Journey 01 - Big O and Arrays
category: "tutorial"
cover: chennai-img.jpeg
author: kush daga
---

Hello everyone!
Here is a subtle attempt of me trying to tag you guys along my journey of starting to learn Data Structures and Algorithms. Now this series is not something that is guaranteed to get you a job, in-fact I'm not even studying DSA to get a job, I mean yeah that is an added benefit maybe, but I'm studying this for my love of CS.

## This isn't my first time!

This isn't my first time trying to learn DSA, I've tried it so many times before as well. It always ends up with me getting bored or me not really wanting to do it. I had no real motivation! But this time I though of something different, this time I want to do it because I want to get my basics right. I have seen many people doing a 2 month course and then starting with amazing jobs in amazing companies but with *no real projects*, and that is what led me to think every time that I don't wanna follow this path of learning! But I can't change the system neither should I fight for it at this time, I am confident that I love developing projects, making things that matter and continuing my love for computer science!

So here I am with another attempt at getting my hands dirty with DSA and not just focusing on Competitive Programming aspect of this, rather the learning aspect for the same. I wanna get into this field because I believe every computer science student or engineer should have some basic familiarity with this topic. I've started a course on Udemy by Andrei who is a great teacher and I had also done his web development course, and now have decided to track my learning and putting out a blog and (maybe) a youtube video explaining what I learnt from his teaching.

## What is good code?

Soo, let us get into the topic and ponder upon this small thought. `What is a good code?` 

Well as I understand it, a good code is subjective to the organisation, the coder, the contributors, etc. But if we generalize it to fit the most cases, a good code comprises of maily two things:

- Readable
- Scalable

This means that if your code is Readable and Scalable it can be categorised into good code. So how do you achieve these things? In this series of articles I'll be focusing on the scalable aspect of a code, you can find many resources on the internet for writing readable code as well. Now, for the scalable aspect of a code, let's start with the basics.

## The Big O Notation

Before diving into this, lets first realise why we need this notation? 

### Why Big O

Let's assume you and your friend are trying to write a program to let's say find the sum of two integers. Now you write code-1 and he writes code-2, now obviously you want to optimize your code to find the best possible way to achieve your end goal that is sum of two integers in the fastest possible way and it should take minimum memory.

Now you run your code in your pc and get that it gives the result in 50ms (assumption) and your friend runs thier code and says that it took 40ms to give the result. 

> `Which code is faster? You or your friends?`

You might be tempted to answer that your friends code is better because it solved the same problem in less amount of time, but actually, after comparing the codes, you find out that you have the same exact code, then why this discrepancy?

This is because the actual run time of a code is relative to many things, for example how good your CPU is, how much ram you have, how many other apps are running in your pc, etc. And so we come to realise that well, maybe comparing the run times is not the best solution to measure the performance of your codes. And this is the reason why we need a unified or a general way of measuring the performance of our codes keeping in mind that the actual times can be relative.

### So what is Big O

Well, in the terms of a 5 year old

> `It simply means that when we increase our number of operations, how long will the code take and is used to measure this criteria. OR When we grow bigger and bigger with input how much the algortihm slow down?`

As said above Big O is simply a means to measure the performance of your code, now Big O can be classified into different categories, O(n) (Called as Big O of N), O(1), O(n^2), etc.

Big O is the worst case of a program. There are 4 rules that have to be followed while finding out the Big O or the time complexity of a program

- Worst case

  - This means that we will focus on the worst case of an algorithm, for example, 

    `function findNemo(array) {
      for (let i = 0; i < array.length; i++) {
    ​    if (array[i] === "nemo") {
    ​      console.log("Found Nemo");
    ​    }
      }
      console.log("The call to this function took", t1 - t0, "Milliseconds");
    }`

    

- Drop the constants

- Different Terms for inputs ( that means if two for loops for two variables i and j, then O(m+n)) is the complexity

- Drop Non Dominants (n^2 more imp than n)