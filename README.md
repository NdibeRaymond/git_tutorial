# What is Git ?

Git is the most widely used version control system in the world today. Designed by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds), an enomous amount of projects depend on it for version control.
According to the official git website, 
“git is a [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) distributed version control system designed to handle everything from small to very large projects with speed and efficiency ”
Ok. Now you might be asking, “what is a version control system? And what does distributed mean in this context?”. Let’s go down the rabbit hole a bit starting with “version control system”.

Version control systems are software tools that help software teams or individuals keep track of every change/modification to their software product over time.

A distributed version control system is a type of version control system that doesn’t exist only in one location. This is to say that every member of a software team using git will posses  a copy of the history of all the changes made to the project over time.

## Why is version control important?
Consider this basic example. Assume you are currently at the job seeking stage of your career and you plan on applying to 10 different organisations with very different application requirements (maybe organisation 1 requires just a cv and organisation 2 requires both cv and cover letter, etc). You also plan on tailoring the different applications for each organisation. This is the likely scenario that would play out.

You create a folder name company1, and put the cv written for company1 inside the folder.

Then you create a second folder named company2, with cv and cover letter for company2.

Then you create a third folder, and a fourth, and a fifth, each containing varying number of files. You can easily end up having more than 50 files flying around everywhere, at which point, it becomes really painful tracking the changes made to these files. Keep in mind that we only assumed you are the only one working one these files. What happens if you ask a friend to help you review these application documents and maybe make corrections?

This is a very basic example and a relatively harmless one. When you are working with software code-bases, the stakes are a whole lot higher. It even gets nastier when you have many developers working on the same code base, this is exactly the kind out situation where git shines.

#### This tutorial comprises of two parts, the more [theoritical article](https://ndiberaymond.pythonanywhere.com/posts/40/) and the practical exercises that lives on this repository. To get the best out of this tutorial, I designed two exercises to help you fully grasp the concept behind git. 
#### First try to complete the [manual version control exercise](https://github.com/NdibeRaymond/git_tutorial/blob/master/excercises/0_manual_version_control_excercise/README.md), then complete the [git version control exercise](https://github.com/NdibeRaymond/git_tutorial/blob/master/excercises/1_git_version_control_excercise/README.md) in parallel with [this tutorial](https://ndiberaymond.pythonanywhere.com/posts/40/). the tutorial and the the exercises on this repository are designed to compliment each other. With the tutorial being the more theoretical half while the exercises serve as the practical half of the whole tutorial.

#### When you have completed both the theoritical and the practical parts, you might want to check out [this pratical tutorial](https://ndiberaymond.pythonanywhere.com/posts/41) on how to contribute to open-source projects

