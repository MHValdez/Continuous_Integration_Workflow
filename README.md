**\*\* The [actual repo](https://github.com/welchmea/swe_group_workflow) for this project is private per the instructor. Collaborator invite *potentially* available upon request, depending on response from partner who is hosting the repo. \*\***

# Continuous_Integration_Workflow
Portfolio project for Software Engineering II

*The actual repo for this project, containing code, tests, and pull request comments, is private by instructor request.
My notes on my introduction to the CI workflow are provided below.*


## Previous Team Projects

My experience developing software on a team is entirely within the OSU CS BS program. In Introduction to Databases, I had a term project with a partner to make a SQL database and a NodeJS frontend. In Software Engineering I, I completed a term project with a partner in which we each developed an application that required a microservice to function. We were each responsible for developing the microservice for our partner’s application.

For the database project, we chose a bookstore inventory. This required us to develop an entity-relationship diagram and a normalized schema before building the frontend and then incrementally implementing CRUD operations. Our initial design was too ambitious for the time constraints, so we had to pare it back while still meeting requirements. We did not use version control.

For the microservice project, I chose to build a React application that provides an interface for a microservice that converts common units of measure. My partner chose to make a blackjack game that gets play recommendations from a microservice. My role was to develop my conversion interface and a play recommender in coordination with my partner. I also provided API requirements for the converter. We did not run into many problems. At one point my microservice was not handling a specific input case but we sorted that out easily. We never touched each other’s codebases, so version control was simple.

## Working with Continuous Integration

The introduction of the Continuous Integration (CI) workflow filled in knowledge gaps that would have been useful in the database project.

The CI workflow itself did not concern me from the outset. My only concern was with the GitHub interface and whether my group members and I would understand how to use it correctly. Referring to the Git introduction in the course materials and simply experimenting on GitHub alleviated this. This was the first course I’ve taken that formally teaches use of Git and GitHub.

I found code reviews helpful and informative. For my code reviews, I took the lessons of the previous code review assignment to heart: I provided constructive feedback with code examples and refactoring suggestions when appropriate. Because my time zone was two hours ahead of the rest of my group, I made a habit of reviewing any pending pull requests in the mornings to remove blockers for forward work.

I made my pull requests using a modified Test-Driven Development (TDD) model. I created a branch on which I incrementally created tests and the code to pass them until I completed a specific sub-function. Then I made my commits and a pull request.

I was responsible for the my_datetime function. As such, I made my first three pull requests when my
code correctly returned years, then months, and then days not accounting for leap years. I made the
final pull request when I had implemented leap years.

My group interpreted the daily commit requirement to mean every day on which code is actually
written. We informed each other when we would not be working due to other obligations. The policy
helped maintain momentum and ensured we only needed to review bite-sized chunks of code. It made
the process smooth. We had no trouble committing our changes on the days we worked.

As a group, we did not require that everyone adhere to a strict TDD process. We felt that is generally
helpful for catching edge cases but potentially too constricting. One group member used tests that
needed to be updated to pass after more features were implemented. I noted this in a review and the
group member handled it in a subsequent pull request. I did attempt to follow TDD in my local
development process but, in one case, decided to improve some previously merged tests rather than
write new ones. In another case, I deleted tests for dates prior to the Unix epoch when I realized it was
outside scope. This confirmed our concerns about strict adherence.

Using CI to manage non-trivial version control on GitHub was a new experience for me. I think handling
pull requests and merge conflicts in a group setting prepared me for real-world software development
in a way that was unique in this program. I like to think I was already a pretty good team member going
in; I hope my group feels that way. I also feel I grew as a mentor. My group members were both very
diligent, but it was clear they had less coding and Python experience than me. I was able to provide
constructive feedback to help them simplify their code. The instruction in this class helped me do it
more effectively.

## Lessons for the Future

The CI workflow ensures that code reviews are small enough in scope so that they are not
overwhelming. It also requires merged code to meet a minimum standard. The review process has the
added benefit of providing training and mentorship opportunities to developers.
Mandatory code review provides quick feedback on coding best practices. A developer can learn how to
make code more efficient and readable. They also may be made aware of helpful standard library
functions, unintuitive edge cases, and optimal algorithms.

Our development process used a modified version of TDD that allowed for limited test revision. Even in
this more relaxed form, it ensured that we systematically met all requirements from the specification
and accounted for edge cases. Without it, less obvious issues could easily slip through the cracks.
Maintaining a robust test suite ensured no group member was ever attempting to commit code that did
not meet a minimum standard as defined by the specification. Without the tests, it would increase the
likelihood of introducing multiple bugs that could interact in unpredictable ways.

Familiarity with software development processes and workflows is some of the most important
knowledge I’ve gained in this program. I will be sure to take it with me going forward.
