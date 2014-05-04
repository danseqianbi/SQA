###How to Ensure the Quality of a Software System###
    Lufei 13126112  danseqianbi@gmail.com
    
##Background## 

  - I have learnt Software Quality Asurance this semester
  - I an working as a project intern in Amazon and have a little practice of QA
  - I will talk about how to ensure the quality of a software system in short
  
##main points##

  - Move QA before coding 
  
That’s right.  We are assuring quality of the whole result, not just the code.  If we code the whole thing, but the quality of the design or analysis wasn’t spot-on, we have a problem.  QA starts with analysis and goes through deployment and operations.
 
  - Unit testing vs. Full system testing 
  
Everyone is so caught up with unit testing and TDD, but full-system testing is the only type of testing that gives close to the coverage the system will experience in a production environment.  If you aren’t doing any type of automated testing, start with full-system testing, not unit tests.
  
  - Get to production quick, before the software is finished (ok, this is a point I wish were in the article) 
  
I’m actually expanding on it right here, but you will never have as clear a picture of whether something works until it it goes to production.  Until then, there is a risk that it will fail.  Get to production quick.  Sometimes, it seems that the type of problem or system just won’t work with an incremental rollout.  The hard problem to solve is how to not solve the whole problem right away.  How do we solve a piece of it quickly, but fully solve it.  In some cases, an incremental production rollout might be incremental by feature.  In others, it may be incremental by user group.  Still in other cases, live pilots may be appropriate.  In any case, old and new systems will need to be integrated.
