---
title: Standing on the shoulders of regularly sized people
date: "2019-11-04"
description: A non-comprehensive thought trail of why BSD license and the like are great.
tags: ["typeorm", "sequelize", ""]
---

Today I made the tough decision to switch ORM's (Object relational mapping) from [Sequelize](https://github.com/sequelize/sequelize) to [TypeORM](https://github.com/typeorm/typeorm). Well, it wasn't _that_ tough, but I was in purgatory for a moment. I couldn't decide the better option for myself and my project. Eventually TypeORM ~~slaughtered~~ gently put my indecision to rest.

How? You ask.

Well, I'm glad you asked! It basically came down to two things:
1. TypeScriptness
2. Automated migrations

But Sequelize, you may be wailing, has TypeScript! Indeed it does but it seems to be an after-thought. Who can blame the contributors for this? After all the first release of Sequelize was back in [2014](https://github.com/sequelize/cli/releases?after=v0.2.2), over 5 years ago. Typescript on the other hand was released [7 years ago](https://en.wikipedia.org/wiki/TypeScript) so how can we expect - wait a minute 7 years ago!? Typescript was around __before__ Sequelize! It was even at v1.3.0 in November 2014.

Geez, come on Sequelize peeps why didn't you start building it in Typescript then!?

Still, I don't blame them. Back in 2014 whodda thunk a superset of JavaScript created by Microsoft would've taken the developer world by storm. They probably weren't seen as a bastion of open source goodness. Well, not that I know of. I'm no authority I wasn't even thinking of getting into web development 5 years ago!

In anycase, Sequelize started including their own TypesScript definitions in v5 and 98.9% of it is written in JavaScript. Ew! Whereas only 0.3% of TypeORM is written in JavaScript and the rest is written in the beautifully delicious TypeScript! I'm not sure if it has anything to do with the fact that TypeORM's very first release was in [2016](https://github.com/typeorm/typeorm/releases?after=0.1.0). I haven't looked deeply enough to see if they started to use TypeScript at that point, the version of which would've been v2.1.0. That's the start of a major jump in versions.

Regardless, I don't have to do any fluffing around to get TypeScript to work with TypeORM - it works out of the box. That's great! Whereas Sequelize I had to find examples and fiddle around and be confused about whether to use the `.define` or `.init` and the cli creating models as `.define` but majority of examples being in `.init` and... well, it was just a _hassle_. We all know developers want to minimise hassle at all costs.

This