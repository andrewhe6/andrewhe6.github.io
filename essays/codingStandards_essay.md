---
layout: essay
type: essay
title: "First ESLint Experience"
# All dates must be YYYY-MM-DD format!
date: 2024-09-26
published: false
labels:
  - Software Engineering
  - Learning
  - Coding Standards
---

## What is ESLint?
ESLint is a JavaScript code analysis tool that helps programmers improve their code by highlighting syntax and formatting errors. It may sound annoying (and sometimes it is) but I think it is an overall beneficial tool for software engineers. Firstly, it can quickly inform you of any syntax typos in your code. Added a colon ot the end of a line instead of a semicolon? ESLint got your back! Some people might find it a pain having to constantly find a fix for the red line just to please the ESLint gods, but I think it is helpful for having software engineers develop better coding standards. 

## Why Coding Standards Are Important
Coding standards can be annoying at times but are overall an important software engineering technique. For example, this piece of code follows the ESLint standards:
```
function findSum(num1: number, num2: number): number {
  return num1 + num2;
}
```
For a simple function like this, I will admit that ESLint is a bit overkill. Without coding standards, however, the same piece of code could look like this:
```
function 
fs(n,
m)
{return n+m
}
```
Both code blocks do the same thing and run without error (according to a quick test on JSFiddle), but the first block is a lot more readable. Personally if I had to work with anyone who coded in the style of the second block, I would wonder how the job market has fallen so much that a company would have to resort to hiring someone who writes such horrendous code. Obviously this is an extreme example and no sane person would ever code in the style seen in the second block. However, even 'trivial' implementations of coding standards are pretty important as they create cohesiveness in a program which makes it overall easier to read. For example:
```
for (i=0; i<var.length; i++) 
{
  total+=i;
}

for (index = 0; index < var.length; index++) {
    total = total + index;
}
```
Both loops ultimately do the same thing but if both styles are utilized in the same program, they can seem like two different functions with different purposes at a quick glance. Having a consistent coding standard utilized throughout the whole program lets our eyes flow uninterrupted, making it a lot easier to read. This is especially useful for larger functions and functions that deal with multiple classes, abstract datatypes, and objects, as ESLint will force you to give each variable a type. The best part about ESLint is that all the "nitpicky guidelines" that it enforces is entirely customizable which means you get to choose how much suffering the red lines cause you! 
