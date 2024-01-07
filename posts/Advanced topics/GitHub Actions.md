# 1. Definition

> Github Action is a service provided by Github that helps you automate build, test, etc pipeline. Therefore, Github Action is a <b> CI/CD platform </b> .

***

# 2. Concepts of Github Action
## 2.1 Job
## 2.1.1 Definition

> Job is a unit of processing in an indepent environment. 

In a workflow(as defined below),  jobs are consist of **runs-on** and **steps** properties.
if you are using version of github enterprise, you can customize github action runner.

## 2.1.2 Usages 

Example of job [^1]

```
jobs:
  echo-hello-world:
    runs-on: ubuntu-latest
    name: Echo Hello World Job
    steps:
      - uses: actions/checkout@v2
      - run: echo Hello World!

 ```


---

## 2.2 Workflow 

## 2.2.1 Definition

## 2.2.2 Usages

Example of Workflow [^1]

```
on:
  push:
    branches:
      - main
      - develop
  pull_request:
```

---


# References 

[^1]: https://tech.kakaoenterprise.com/180 