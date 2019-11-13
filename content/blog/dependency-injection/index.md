---
title:
date: "2019-11-13"
description:
tags: ["dependency injection"]
---

Today was full of reading and understanding, at least attempting to understand - I can hear Yoda in the background saying "Don't try, DO". OK, OK! I was doing to understand. My topic for understanding was Dependency Injection. This is a pattern in software development AND web development AND software engineering in which dependencies... are... um... injected... into - but seriously. Dependency Injection (DI) is a pattern in which a object/library/service/etc that is needed for another object/library/service/etc is passed into that object/library/service/etc. I'm not sure it's the most accurate definition, nor the most correct.

To compared DI to other patterns, it is different to a dependency being "found" or "built" by dependent. I'm not exactly sure how the import/require functionality works in modern day JavaScript but it could be that when a JS library/file, otherwise known as a module, is imported/required into another JS file that module is told where it's located. When JS builds the file then all the imported modules are wrapped up together. I've got a feeling this isn't DI as DI involves passing the dependencies a dependent needs to run into it.

Anyway, I think I'm butchering the definition. Check out this [metaphor](https://stackoverflow.com/questions/1638919/how-to-explain-dependency-injection-to-a-5-year-old) over on our beloved Stack Overflow. This is a much better explanation of DI. I couldn't explain it to a 5 y.o like this, so yes, I don't really understand what it's all about. I still feel I don't fully understand it even after reading [this](https://medium.com/@Jeffijoe/dependency-injection-in-node-js-2016-edition-f2a88efdd427) and some of [this](https://www.martinfowler.com/articles/injection.html), because it was more theoretical than I wanted at the time.


I've got a sense of what it is about, I got a feeling that I want to implement it in the project I'm working on because I think it'll solve an issue I've got at the moment with the project I'm working on. There are functions, which I could turn into classes, that are not easily being passed into other classes.