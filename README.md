# Challenge: development

## Introduction

GitHub is a social network of programmers that has an interesting functionality that allows you to ["star" other users repositories](https://help.github.com/en/articles/saving-repositories-with-stars). The users activate that just by pressing a button. But it has some limitations when we consider GitHub heavy users.


## Use case

You are an active GitHub user, who is always looking for new projects and enjoying those who are interesting. You would like to be able to add a label or tag to a repository so that it can be found later. For example, you've found a repository called `react` and you would like to add ` javascript` and `frontend` tags to it. Because GitHub does not have this functionality, you want to build a simple system that can help with this task.

## Requirements

- Retrieve starred repositories of a user's GitHub profile.
- Manage retrieved repositories tags (i.e., add, edit, delete).
- Filter repositories by tags.
- Suggestion of tags for repositories.

## User stories

#### 1. Obtain repositories

> As a user, I want to provide my username to retrieve all repositories. I like it so I can add my tags later.

- You should get starred repositories using the GitHub Rest v3 API. Using the v4 API with GraphQL is a plus.
- The information that must be retrieved is: Repository ID, repository, description, HTTP URL, and language.

#### 2. Add tags to repositories

> As a user, I want to be able to add tags to each repository so I can search them later by tag.

- A repository can not have duplicate tags.

#### 3. Search repositories by tags

> As a user, I want to be able to provide a tag and get the repositories that have this tag associated.

- The search should work for queries with strings in half (e.g., by typing `doc`, the` docker` and `documentation` repositories must be returned).

#### 4. Tag recommendation

> As a user, I want to receive tag recommendations for my repository.

- Each repository should receive at least one tag recommendation.

## Exercise

In order to implement the user stories listed above, please, choose just one of the following instructions: back-end, or front-end. If you want to make both, we will consider this an extra point and effort, but it's *not* mandatory.

#### Back-end instructions

- Your REST API must be implemented using JSON.
- Each action must have its specific route respecting the convention of `http verb` and `status code`.
- Repositories and their tags must be persisted at a local bank.
- Using Docker to configure the environment is recommended, but not mandatory.

#### Front-end instructions

- The user interfaces (UI) must follow the design provided below:
1. [home](https://github.com/Danielwsx64/challenge-development/blob/master/wireframes/01.png)
2. [loading](https://github.com/Danielwsx64/challenge-development/blob/master/wireframes/02.png)
3. [repositories list](https://github.com/Danielwsx64/challenge-development/blob/master/wireframes/03.png)
4. [manage tags](https://github.com/Danielwsx64/challenge-development/blob/master/wireframes/04.png)
5. [filter by tags](https://github.com/Danielwsx64/challenge-development/blob/master/wireframes/05.png)
- Repositories and their tags must be persisted in the user's local storage.
- The use of libs such as Redux, Vuex or Flux is recommended, but not mandatory.
- Using Docker to configure the environment is recommended, but not mandatory.

## What we will evaluate

We want to evaluate your ability to deliver a simple product with sufficient documentation for other developers to actively contribute to the project later.

#### For both back-end and front-end exercises

1. `README.md` well written, short and with the commands needed to run the application.
2. Well written code, clean and cohesive.
3. Implementation of the solution.
4. Automated testing (i.e., coverage of the tests).
5. Linter/static code analysis.

#### For back-end exercises

6. RESTful API design, correctly using the `HTTP` verbs and the proper `Status Code`.
7. API documentation using the web (e.g., [Blueprint](https://apiblueprint.org/), [Swagger](https://swagger.io/), [Postman](https://www.getpostman.com/), etc.), not being able to use `pdf`, `txt` or any other file format.

#### For front-end exercises

6. Knowledge in Javascript, HTML5 and CSS3.
7. Ability to implement the screens exactly as it is in the wireframes provided, considering the position of the elements on the screen.

## Programming language and/or frameworks

You may choose the technology of your choice. Only for your information, we disclose the following technologies that we are used to develop.
- Elixir
- Ruby on Rails
- Python
- React
- Flutter

## How to share your exercise with us
1. Create a `README.md` file describing how to configure the project, containing the commands that must be run to run the software and tests.
2. Open a new Pull Request to the `master` branch of the private repository the we have provided through our admin.
3. If you have made use of any Linter (esling, rubycop, creed, etc.), send the file together with the project.
