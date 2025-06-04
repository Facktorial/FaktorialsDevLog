---
layout: post
category: general
slug: struggle programming
title: Hmmm, typical workflow, oh shiiiit, here we go again...
---

Let's say, we are working hard[^1] on finishing our third custom game engine, as every proper programmer should, and then we realize -- what the hell I am doing? This shit again??? The same behavioral pattern[^2] (last time we swore we'd never do it again, that next time we'd be more careful) occured:

- Hmmm, lets focus on rendering pipeline. I would be nice to see something on screen finally.
- But, it's good idea start working on ECS, good designed, good optimized, it will be a solid foundation I can rely and build upon as develompent progresses.
- This seems as I will finish skeleton of my ECS in no time, but,... wait a minute ... for optimized ECS[^3] is killer using std::vector, there will be better fitter container
- So, I am writting my implementation of PagedVector[^4] and sudenly realize: I need my custom verbose implementation of zip function to iterate through multiple containers[^5].
- Hmm, this is another relatively common feature, it should not be in my game engine project. It should be in my own templated STL library.
- When I am creating my custom library, I should made it well and fill some technical gaps in my skills.
- I got clang-tidy, clang-format, docker, CI/CD, only conan is missing now.
- When I created multiple libs. I should learn what is plugin, and how make them with conan. And why.
- WHY THE FUCK I am writing a Plugin manager? I though I want just create simple game.
- I should learn from my mistake, again.
- Now I am working out, how create devblog on github pages and fine tunne this post.


How deep the rabbit hole goes?[^8]

Do you premature optimize as well?

---
{: data-content="footnotes"}

[^1]: okay, we believe we are working hard.
[^2]: last time we swore we'd never do it again, that next time we'd be more careful.
[^3]: which makes different only when we got relly scaled up data
[^4]: [PagedVector](https://peterino.com/Paged%20Vector.html) is data structure that under the hood relies on const size arrays.
[^5]: Zip function is not in C++20 standard, but will come in C++23.
[^8]: I stole and canibalized this example, even next sentence. By the way this is a longer footnote and i think it is still pretty cool, even prettier than shortier ones even though it does not say anything useful but whatever.
