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

> As a user, I want to provide my username to retrieve all repositories so I can add, edit or delete my tags later.

- You should get starred repositories using the GitHub Rest v3 API. Using the v4 API with GraphQL is a plus.
- The information that must be retrieved is: repository ID, repository name, description, HTTP URL, and language.

#### 2. Add tags to repositories

> As a user, I want to be able to add tags to each repository so I can search them later by tag.

- A repository can not have duplicate tags.

#### 3. Search repositories by tags

> As a user, I want to be able to provide a tag so I can get the repositories that have this tag associated.

- The search should work for queries with strings in half (e.g., by typing `doc`, the` docker` and `documentation` repositories must be returned).

#### 4. Tag recommendation

> As a user, I want to receive tag recommendations for my repository.

- Each repository should receive at least one tag recommendation.

## Exercise

In order to implement the user stories listed above, please, **choose one of the following instructions: back-end, or front-end**. If you want to make both, we will consider this an extra point and effort, but it is *not* mandatory.

#### Option 1: Back-end instructions

- Your REST API must be implemented using JSON.
- Each action must have its specific route respecting the convention of `http verb` and `status code`.
- Repositories and their tags must be persisted at a local bank.
- Using Docker to configure the environment is recommended, but *not* mandatory.

#### Option 2: Front-end instructions

- The user interfaces (UI) must follow the design provided below:
1. [home](wireframes/01.png)
2. [loading](wireframes/02.png)
3. [repositories list](wireframes/03.png)
4. [manage tags](wireframes/04.png)
5. [filter by tags](wireframes/05.png)
- Repositories and their tags must be persisted in the user's local storage.
- Using Docker to configure the environment is recommended, but *not* mandatory.

## What we will evaluate

We want to evaluate your ability to deliver a simple product with sufficient documentation for other developers to actively contribute to the project later.

#### For both back-end *and* front-end exercises we will evaluate if:

1. `README.md` is well written, short and with the commands needed to run the application.
2. The code is well written, clean and cohesive.
3. Implementation of the solution is working as expected.
4. There is automated testing (i.e., the coverage of the tests).
5. There is linter/static code analysis.

#### For back-end exercises we will evaluate if:

6. RESTful API design is implemented, correctly using the `HTTP` verbs and the proper `Status Code`.
7. API documentation is using one good web tool (e.g., [Blueprint](https://apiblueprint.org/), [Swagger](https://swagger.io/), [Postman](https://www.getpostman.com/), etc.), and not `pdf`, `txt` or any other file format.

#### For front-end exercises we will evaluate if:

6. There is good usage of Javascript, HTML5 and CSS3.
7. The screens were implemented exactly as it is in the wireframes provided, e.g., the position of the elements on the screen.

## Programming language and/or frameworks

You may choose the programming language of your preference.

## How to share your exercise with us
1. Create a `README.md` file describing how to configure the project, containing the commands that must be run to run the software and the tests.
2. Open a new Pull Request to the `master` branch of the private repository that we have invited you to contribute.
3. If you have made use of any Linter (esling, rubycop, creed, etc.), send the file together with the project.
