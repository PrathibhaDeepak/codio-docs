---
title: Stack planning


---

The following applies to project units rather than books. Books require less thought as a book only has one box associated with it and the book unit will takes its stack setting from the book.

You should be familiar with the concept of [a stack](/project/stacks/stack-overview) before creating CS coursework.

# Minimize the number of stacks
It is important to think about the [stack or stacks](/project/stacks/stack-overview) that your course uses. You should avoid creating a new stack for each unit. There are very few cases where this is needed. If you unnecessarily create new stacks for each unit, you will be be less efficient and waste unnecessary time with stack builds.

You should look to use as few stacks as possible, ideally just one, and use that stack for all units. There are perfectly valid exceptions, but this is the rule.

# Single stack example
To illustrate a single stack situation, let's assume you are teaching a course "Programming in Java". You could either use our default Java stack or you start with the Java stack and then add additional tools so it has all the components you require to teach all parts of your course.

Whether you have created your own stack or used a default one, you would then point all your units to that one, same stack.

If, as you create more units in your course, you find you need to install more tools, then you should [update the stack with a new version](/project/stacks/update).

By default, when you choose a stack for your new unit, it will point to the latest version. So if the underlying stack is updated from any location at all, then any unit that uses that stack will automatically be set to use it. Students who are using a unit in a class will also automatically use the latest version when it is updated.

It follows that you should be very careful when pointing to a specific version of a stack, rather than the latest version. If you do this, then you will need to update all units that are not set to use the latest version.


# Multiple stack example
Let's say you are teaching a course "Introduction to Programming" and it has 3 modules "Java", "Python" and "Haskell" and each module contains a good number of units. In this case, you could still choose the single stack approach, but you would need to install all three languages and their toolsets and then create a stack from it.

A simpler approach would be to use three separate stacks, one for each language. You set the units for each language to point to the appropriate language stack.

Other than that, the principles described above still apply.

# Switching stacks
It is possible to change the stack for a unit. This can be done from either the listing or from within the IDE. However, if this change were to be needed for all units then you would have to repeat this for each unit individually.

It is therefore highly recommended that you start with a stack and stick with it wherever possible.

# Stacks not owned by you
If you were to use one of Codio's default stacks then you are not able to update these yourself as you don't have permissions. However, you might want to start off with, say, the Java stack and then install new components.

In this case, you should plan this ahead of time. You would

- first create the unit from Codio's Java stack
- install your components
- create a new stack from your unit ([in the IDE](/project/stacks/update#stackide) or when you [publish](/courses/units/publish))
- make sure your stack is switched to that newly created stack

You now own this stack and so you can update whenever you like down the line. When you create new units, you would then choose this new stack.

# Use Latest Version
When you assign a stack to a unit, it will be set by default to the **Use Latest Version**. If you view the stack settings from the IDE (**Project-Stack Settings**) or from the 3 blue dots menu, you will see that this is the default.

<img alt="Unit stack settings" src="/img/stacksettings.png" class="simple"/>

Understanding what **Use Latest Version** means is important. When you work with a unit as a course author, that unit is actually using a fixed version. It does not automatically switch to the latest version each time a new version of a stack is created. This could be dangerous as switching a stack resets everything outside the workspace folder. If you want to update to the latest version then you need to go to the stack settings dialog and press the save button.

Where **Use Latest Version** is useful is when you assign a course module and its units to a class. In this case, students who have not yet started a unit **will** get the latest version of the stack.