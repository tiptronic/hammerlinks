# Using Symlinks in Hammer

With the help of some simple symlinks you can enhance your productivity quite a bit by creating common assets used across your projects.

## What is it good for?
Lots of times I use quite some assets, libraries, utilites, etc... commonly in various projects. This requires me to either copy a generic project and remove what's not needed, or create a new project and drag in my required files. This is cumbersome and boring.

When I change one (or more) of these commonly used files, I must go through all my projects and change/replace the changed files there as well. This is even more boring and error-prone.

With the help of some symlinks we can easify this process, by putting commonly used files into a shared folder and use these files (from within Hammer) for all of our projects.

## How does it work?
Let me show you the power of this technique by a simple example:

1.	First we create 2 projects right from within Hammer (of course, you can create 2 projects manually as well)
2. For better readability I renamed the projects to p_ONE and p_TWO
3. Create another folder 'common' in the same folder as the two projects
3. Open up your terminal and type in these lines

```
$ cd /Users/andy/hammertest/p_ONE/assets/js
$ ln -s /Users/andy/hammertest/common/js/jquery-1.8.3.min.js
$ ln -s /Users/andy/hammertest/common/js/app.js
```

