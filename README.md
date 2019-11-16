# Coding Challenge

## Summary

Design and implement a prototype job automation system with a simple web front-end.

This challenge has two goals:

- It helps us to understand what to expect from you as a developer. How do you write production code, how you reason about design and how you communicate when trying to understand a problem before you solve it.
- It helps you get a feel for what it is like to work at BlueStone, as this challenge aims to simulate our workflow.

## Requirements

The goal is to implement a job automation system that is able to execute jobs concurrently and a web client that supports creating jobs, executing jobs and viewing job status in real time.

### Client

Here is a list of features that the web client should support:

- Create a **Task Blueprint** with name. A task blueprint can be used to create a task instance, which is the building block for a specific job.
- Create a **Job** with name and associated task instances. A user can select a set of tasks from all available task blueprints and order them in any sequence. Modification to a job and its task sequence is not allowed after the job was created.
- Display a list of all created jobs with associated task instances.
- Start jobs. It should support running multiple jobs in parallel without breaking the application.
- A user can easily identify the status of a job or a task in real time. For example, status can be *idle*, *running* or *finished*.

To illustrate what a job list might look like:

```
Job 1: [T1 -> T2 -> T3]
Job 2: [T3 -> T2]
Job 3: [1]
```

In the above example, task instance `T1` was created from task blueprint `B1` after `Job 1` was created.

### Server

The server should be able to handle client's requests as mentioned above.

You may wonder what exactly a given task is running against? It does not really matter for this project, so, for simplicity, each task does nothing but sleeps for 3 ~ 5 seconds at random to simulate it's working on something.

## Guidance

### Interview Process

We understand that the interview is a two-sided process and we’d be happy to answer any questions!

Before writing the actual code, we encourage you to **create a small design document** and share it with the team through email. This document should consist of key design approaches and key trade-offs. Please avoid writing an overly detailed design document. Use this document to make sure the team can provide design feedback and demonstrate that you have investigated the problem space to provide a reasonable design.

After we approved your design, you can start implementation. Once you finished the project, please submit your solution via email.

If you submission is accepted, we will schedule you a phone interview with the team. In the case of rejection, please don’t be discouraged. You are welcome to take another challenge at a later time.

### Trade-offs

It is important to write as little code as possible. Otherwise, this task could consume too much time and the overall code quality will suffer. It is OK and expected if you make reasonable assumptions and cut corners. Be sure to add TODOs or comments to demonstrate that you’ve spent time thinking about this problem and provide a clear path to a solution.

Here are some trade-offs that will help you to spend less time on the task:

- Do not implement a system that scales or is highly performing. Instead, communicate the performance improvements you add in the future.
- High availability. It is OK if the system is not highly available. Write down how you would make the system highly available and why your system is not.
- Do not try to achieve full test coverage. This will take too long. Implement one or two test cases for key components to demonstrate your approach to testing.

### Delivery

This project can be implemented in any language/framework/technology of your choice.

Once you finished the project, please deploy your project for demo purpose, make sure to populate some jobs in the demo. 

Finally, email your solution and the live demo URL to the team.

### Evaluation

We want to be as transparent as possible on how we will be evaluating your submission. The following list provides a description of different areas you will be evaluated on:

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

Because this project simulates day-to-day work which involves design, implementation, code review and feedback, there will be a certain amount of communication overhead for sure. And we understand candidates may have different levels of availability, so we don't impose a hard deadline for this project. We usually expect a working deliverable within two weeks, so please let us know if you need extra time.

## Asking questions

It is OK (and encouraged) to ask the interview team questions. Some folks stay away from asking questions to avoid appearing less experienced, so we provided examples of questions to ask and questions we expect candidates to figure out on their own.

This is a great question to ask:

> Is it OK to put the secrets in the repository for the purposes of demo? I will add a note that we will auto-generate secrets in the future.

It demonstrates that you thought about this problem domain, recognize the trade off and save you and the team time by not implementing it.

This is the type of question we expect candidates to figure out on their own:

> What version of XXX should I use? What dependency manager should I use?

We expect candidates to be able to find solutions to common non-project specific questions like this one on their own. Unless specified in the requirements, pick the solution that works best for you.

## Contact

Email: careers@bluestone.live

Finally, THANK YOU for taking your time to take the challenge. We understand that your time is valuable and we really appreciate it!

Have fun!
