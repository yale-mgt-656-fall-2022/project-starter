# Project starter

Ahoy! This is the project starter. I've done some
of the hard parts for you. Good luck.

## Building the project

Run `go build -mod vendor` to compile your project and then
run `./classproject` or `./classproject` on Windows
in order to run the app. Preview the app by visiting
[http://localhost:8080](http://localhost:8080) if you're
running it locally. Or, preview using the URL provided
by cloud9 if you're running on cloud9, natch.

## Deploying to Heroku

I included a `go.mod` file and a `Procfile` so you
should have no trouble deploying to Heroku. Of course,
your team should only have one Heroku app (usually)
and you should all be "collaborators" on it. You're
welcome to deploy to other places too---I don't care.

## What is here

| File                      | Role                                                                                                                      |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| ./README.md               | This file!                                                                                                                |
| ./server.go               | Entrypoint for the code; contains the `main` function                                                                     |
| ./routes.go               | Maps your URLs to the controllers/handlers for each URL                                                                   |
| ./event_models.go         | Defines your data structure and logic. I put in a few default events.                                                     |
| ./index_controllers.go    | Controllers related to the index (home) page                                                                              |
| ./templates.go            | Sets up your templates from which you generate HTML                                                                       |
| ./templates               | Directory with your templates. You'll need more templates ;P                                                              |
| ./templates/layout.gohtml | The "base" layout for your HTML frontend                                                                                  |
| ./templates/index.gohtml  | The template for the index (home) page                                                                                    |
| ./static.go               | Sets up the static file server (see next entry)                                                                           |
| ./staticfiles             | Directory with our "static" assets like images, css, js                                                                   |
| ./Procfile                | A file that helps heroku run your app                                                                                     |
| ./go.mod                  | [Go modules file](https://www.kablamo.com.au/blog/2018/12/10/just-tell-me-how-to-use-go-modules). Lists our dependencies. |
| ./go.sum                  | A "checksum" file that says precisely what versions of our dependencies need to be installed.                             |
| ./vendor                  | A directory containing our dependencies                                                                                   |

## Automatic reload

If you want your app to reload every time you make a
change you can do the following. First
install reflex with `go get github.com/cespare/reflex`.

Then, run

```
~/go/bin/reflex -d fancy -r'\.go' -r'\.gohtml' -s -R vendor. -- go run *.go
```

or something like that. Look at the reflex documentation. Automatic
reload is pretty rad while developing. As a general rule, developers
want to let computers do what computers are good at (tasks that can be automated)
so that they, the developers, can focus on what they are good at: the
logic of the product.

## Other info

Information about the class final project is distributed between
a few places and I apologize for this. You can find information
about the project in the following places:

- This page (which you're likely looking at in your own repo)
- The sprint-1 assignment page:
  [656](https://www.656.mba/#assignments/project-sprint-1)
- The "about" repo for the class:
  [https://github.com/yale-mgt-656-fall-2021/about/blob/master/class-project.md](https://github.com/yale-mgt-656-fall-2021/about/blob/master/class-project.md)
- The grading code:
  [https://github.com/yale-mgt-656-fall-2021/project-grading](https://github.com/yale-mgt-656-fall-2021/project-grading)
- The reference solution
  [http://project.solutions.656.mba/](http://project.solutions.656.mba/)
- My comments in class
