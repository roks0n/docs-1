---
title: "Clean Code & Tests"
---

# Clean Code & Tests

[[toc]]

## Introduction

While the following guidelines are not an absolute requirement or need to be enforced by tools, it is a recommendation based on what we have been trying to do in our projects lately.

## Clean Code

Clean Code is as important as separation of concerns and testability when building an application.

Only through Clean Code you will achieve an application that is easy to navigate, reduces complexity and can be maintained by new and seasoned developers without losing time and money.

The core characteristics of a clean code are the following, you should aim to meet as many of them with your code as possible.

1. Clean code should be elegant, logical and pleasing to read since it is written by developers for developers, your code should reflect this. **Another person is maintaining the code you have written, not a computer. Always keep that mind.**

2. Clean code should be focused, meaning every class, function or module should only be concerned about a single responsibility. **The result of this will be clean, testable code with minimal to no duplication. **

3. Clean code should be taken care of by all developers, as another developer before has taken the time out of their day to keep it simple in order to make the next developers life easier. **Making use of modern development patterns and paying attention to seemingly unimportant things like formatting or variable naming will help you to achieve this goal.**

## SOLID Code

In order to achieve more understandable, flexible, maintainable and testable applications you need to have a clear **Separation of Concerns** in every part of your application.

The [SOLID](https://en.wikipedia.org/wiki/SOLID) pattern comes from the realm of object-oriented programming but applies the same to [functional programming](https://softwareengineering.stackexchange.com/a/171534) as it is just a concept of how to design & build applications.

Here is a quick TLDR to sum SOLID application design up:

1. Each Entity should have a single responsibility.
2. Each Entity should be able to extended, not modified.
3. Each Entity should be replaceable by a custom implementation without breaking the application.
4. Each Entity should follow a contract and always return the same output, no matter the implementation.
5. Each Entity should be as loosely coupled as possible.

## Test Suites

Writing a test suite for your application is detrimental for the maintainability of your application for future developers.

A test suite will make sure that everything is working as intended without you having to manually start the whole application just to test that one small change you made to a database model. **A good test suite will save you time and resources long term, it does not slow down development.**

Try to keep your naming conventions consistent and readable because keep in mind, code is maintained by people, not computers.

You should aim for a high coverage of business critical parts of your application and for at least sufficient enough coverage of utilities and smaller working parts to be confident that any future changes are caught by your test suite which results in failure.

_If you are working on a JavaScript project we recommend you to use https://facebook.github.io/jest/ and follow the `it('should ...')` naming convention._
