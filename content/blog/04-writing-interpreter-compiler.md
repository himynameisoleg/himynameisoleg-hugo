---
tags:
  - blog
  - ultralearning
  - interpreter
  - compiler
title: "From Zero to Compiler: Lessons Learned by Doing"
author:
  - Oleg Perchyk
date: 2025-02-12
---

## Intro

I've noticed that almost every book I read, new restaurant I try, or video game I play is usually based on someone's recommendation. In the data science world, we can build recommendation engines using a technique called "Collaborative Filtering" to help make predictions when the data we have is limited. The gist of it is: "If I like something and I'm into similar things as you, then I must surely like your recommendations!" And how do we do that? Well, we won't go into that here, but since you asked... "we simply need to create a similarity matrix, train a model, fine-tune a few hyperparameters, and bada-bing bada-boom: we now have a model that can make some half-decent predictions..." Just kidding. This took me the better part of a year to learn during grad school, where I had an awesome thesis supervisor (shoutout to Professor Lizi!).

So, recommendations… While deep down a YouTube rabbit hole, I was recommended a pair of software engineering books written by Thorsten Ball: *Writing an Interpreter in Go* and *Writing a Compiler in Go*. Both are well-respected yet approachable technical books, and my interest was piqued. The thought of writing a programming language from scratch—so cool! These books' claim to fame is that they are not overly theory-heavy, very approachable, and hands-on. As someone who loves multimodal learning (arguably the best way to learn), I was immediately drawn to the idea of getting my hands dirty by writing interpreters and compilers.

## More Than Just Writing a Programming Language

I'm not going to spoil the fun and outline everything I learned from the books (you should just [grab the books](https://interpreterbook.com/) and find out for yourself). Instead, I want to explore some of the more subtle and nuanced lessons I picked up while reading and applying what I learned.

![interpreter-compiler-books](../../images/blog/interpreter-compiler-books.jpg)

These books follow a common pattern: the author introduces a topic, we write some Go code, and then he explains what we just wrote. Things intentionally break, and we go back and fix them. We write tests, watch them fail, fix our code, and move on to the next idea. Sound familiar?

## Actually Doing Test-Driven Development

For most of my career, TDD has been just a theoretical "nice to have"—something you read about in blogs or from Extreme Programming. Everyone recommends it, but no one actually does it in practice because, well... deadlines, capacity, budgets, etc. I remember being on a project where we did some after-the-fact unit testing just to bring our code coverage up to an acceptable level. We all knew this wasn't TDD. It's always harder to write tests after the fact. You can't truly appreciate the value of TDD until you write tests first, build enough confidence in your codebase, and then have them save you from breaking a downstream part of your system. *Writing an Interpreter in Go* and *Writing a Compiler in Go* did a great job of getting me into a TDD workflow—something I've been striving to incorporate into my daily development work.

## The ABCs of Software Engineering

"Always Be Coding." Between 2023 and part of 2024, I moved from an IC role into a technical management role. This year-long hiatus from full-time coding had a couple of side effects. As a manager I spent much less time solving technical problems and much more time solving business, process, and people problems. I noticed my programming skills starting to atrophy after just a few months. As someone who thrives on deep, focused work, I wanted to get back to regular bursts of flow state, and these books were the catalyst I needed to get back into shape.

## Marginal Improvements

I'm a huge proponent of marginal improvements and love eating elephants one delicious bite at a time. Because of how these books are structured—where each chapter feels like an achievement—I was able to chip away at them each day, write some code, throw it up on GitHub, and move on with my day. This practice gave me a sense of accomplishment and motivated me to keep learning something new daily.

## New Technologies

These books are written in Go, and I learned to love writing Go. In the process, I also decided it was time to level up my Vim skills. What started as a simple effort to improve my workflow quickly became a deep dive into customizing LazyVim, configuring LSPs, working with tmux and optimizing my development environment. With this workflow, my daily coding sessions went smoothly, vim motions became second nature and I now use it as my daily driver at work as well!

## Wrapping Up

Diving into *Writing an Interpreter in Go* and *Writing a Compiler in Go* was more than just an exercise in learning about interpreters and compilers—it reignited my passion for coding, improved my workflow, and reinforced the importance of marginal improvements. If you’re someone who enjoys hands-on learning, testing your skills, and deepening your technical knowledge, these books are well worth your time. If you’ve ever thought about writing your own programming language, or if you just want to improve your coding skills, I highly recommend checking out these books. They’re practical, engaging, and incredibly rewarding. Let me know if you’ve read them or if you have any other technical book recommendations—I’m always on the lookout for my next deep dive! Feel free to check out my work on [GitHub](https://github.com/himynameisoleg/monkey-language)!
