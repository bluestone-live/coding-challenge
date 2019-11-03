# Coding Challenge

## Summary

Design and implement a prototype job automation system with a simple web front-end.

## Rationale

This exercise has two goals:

- It helps us to understand what to expect from you as a developer. How do you write production code, how you reason about design and how you communicate when trying to understand a problem before you solve it.
- It helps you get a feel for what it is like to work at BlueStone, as this exercise aims to simulate our day-to-day.

We believe this technique is not only better, but also is more fun compared to the whiteboard/quiz interviews so common in the industry. We appreciate your time and we look forward to hack on this little project together.

## Objective

The goal is to implement a job automation system that is able to execute jobs concurrently and a web client that supports creating jobs, executing jobs and viewing job status in real time.

## Requirements

### Client

Here is a list of features that the web client should support:

- Create a task with name. Tasks are building blocks for a specific job.
- Create a job with name and associated tasks. A user can select a set of tasks from all available tasks and order them in any sequence.
- Display a list of all created jobs with associated tasks.
- Start a job. It should support running multiple jobs in parallel without breaking the application.
- A user can easily identify the status of a job or a task in real time. For example, status can be *idle*, *running* or *finished*.

To illustrate what a job list might look like:

```
Job 1: [Task 1 -> Task 2 -> Task 3]
Job 2: [Task 3 -> Task 2]
Job 3: [Task 1]
```

### Server

The server should be able to handle client's requests as mentioned above.

You may wonder what exactly a given task is running against? It does not really matter for this exercise, so, for simplicity, each task does nothing but sleeps for 3 ~ 5 seconds at random to simulate it's working on something.

## Guidance

### Interview Process

The interview team is assembled in the slack channel and consists of the engineers who will be working with you. You are encouraged to chat to them and ask questions about the engineering culture, work and life balance, or anything else that you would like to learn about BlueStone.

We understand that the interview is a two-sided process and we’d be happy to answer any questions!

Before writing the actual code, we encourage you to **create a small design document** and share it with the team by making a pull request on GitHub. This document should consist of key design approaches and key trade-offs. Please avoid writing an overly detailed design document. Use this document to make sure the team can provide design feedback and demonstrate that you have investigated the problem space to provide a reasonable design.

Fork this repo, split your code submission using pull requests and give the team an opportunity to review the PRs. A good “rule of thumb” to follow is that the final PR submission is adding a small feature set - it means that the team had an opportunity to contribute the feedback during multiple well defined stages of your work.

Our team will do their best to provide a high quality review of the submitted pull requests in a reasonable time frame. You are spending your time on this. We are going to contribute our time too.

After the final submission, the interview team will assemble and vote using +1, -2 anonymous voting system: +1 is submitted whenever a team member accepts the submission, -2 otherwise.

If there is a positive result for submission, we will schedule you phone interviews with each member of the interview team. After the calls, the interview team will vote again using the same voting mechanism.

If there is a positive result for phone interviews, we will collect one/two references and work out the other details. After reference collection, we will send you an offer.

In case of a negative score result, we will contact you and send a list of the key observations from the team that affected the result. Please don’t be discouraged. Our code review process is focused on the submission, not the candidate and we will be excited for you to take another challenge at a later time if you feel you have addressed our comments!

### Code and project ownership

This is a test challenge and we have no intent of using the code you have submitted in production. This is your work, and you are free to do whatever you’d like with it.

### Trade-offs

It is important to write as little code as possible. Otherwise, this task could consume too much time and the overall code quality will suffer. It is OK and expected if you make reasonable assumptions and cut corners. Be sure to add TODOs or comments to demonstrate that you’ve spent time thinking about this problem and provide a clear path to a solution.

Here are some trade-offs that will help you to spend less time on the task:

- Do not implement a system that scales or is highly performing. Instead, communicate the performance improvements you add in the future.
- High availability. It is OK if the system is not highly available. Write down how would you make the system highly available and why your system is not.
- Do not try to achieve full test coverage. This will take too long. Implement one or two test cases for key components to demonstrate your approach to testing.

## Delivery

This project can be implemented in any language/framework/technology of your choice.

Once you finished the project, please share with us a live demo URL with some jobs populated.

### Scoring

We want to be as transparent as possible on how we will be scoring your submission. The following list provides a description of different areas you will be evaluated on:

- The candidate communicated their progress during the interview.
- The candidate outlined the key design points in the design document.
- README provides clear instructions.
- The code has a clear and modular structure.
- The code has a consistent coding style.
- The code provides tests covering key components.
- The code provides clear error handling and error reporting.
- The program builds are reproducible.
- The program is working according to the specification.
- The client-server communication is implemented in a secure way.
- The web user interface is easy to use.
- The candidate demonstrates ability to handle and apply feedback.

### Timeline

Because this project simulates day-to-day work which involves design, implementation, code review and feedback, there will be a certain amount of communication overhead for sure. And we know candidates may have different levels of availability, so we don't have a hard deadline for this project. But we expect a working deliverable within two weeks assuming both you and the interview team working actively on this project. Don't worry if you need more time, just let us know!

## Asking questions

It is OK (and encouraged) to ask the interview team questions. Some folks stay away from asking questions to avoid appearing less experienced, so we provided examples of questions to ask and questions we expect candidates to figure out on their own.

This is a great question to ask:

> Is it OK to put the secrets in the repository for the purposes of demo? I will add a note that we will auto-generate secrets in the future.

It demonstrates that you thought about this problem domain, recognize the trade off and save you and the team time by not implementing it.

This is the type of question we expect candidates to figure out on their own:

> What version of XXX should I use? What dependency manager should I use?

We expect candidates to be able to find solutions to common non-project specific questions like this one on their own. Unless specified in the requirements, pick the solution that works best for you.

Finally, THANK YOU for taking your time to take the challenge. We understand that your time is valuable and we really appreciate it!

We wish you good luck!
