# Sample Website
This is a sample website made by Steven Callioux as part of [*Learn Enough™ Git to Be
Dangerous*](https://www.learnenough.com/git-tutorial), possibly the greatest
beginner Git tutorial in the history of the Universe. You should totally [
check it out](https://www.learnenough.com/git-tutorial), and be sure to [join
the email list](https://www.learnenough.com/#email_list) and
[follow @learnenough](http://twitter.com/learnenough) on Twitter.
After finishing *Learn Enough™ Git to Be Dangerous*, you'll know enough Git
to be *dangerous*. This means you'll be able to use Git to track changes in
your projects, back up data, share your work with others, and collaborate
with programmers and other users of Git.
The result in Atom appears as shown in Figure 2.9. As mentioned in Learn
Enough Text Editor to Be Dangerous, Atom includes a Markdown previewer
via the Packages menu item shown in Figure 2.10, which (after resizing the
window) results in the preview shown in Figure 2.11.3
Now that we’ve created the README.md file, we’re ready to add it to our
Git repository and push it up. We can’t just run git commit -am because
README.md isn’t currently in the repository, so we have to add it first:
[website (master)]$ git add -A
(As noted in Section 1.3.1, we could also run git add README.md, but in
most cases we want to add all the new files, so I suggest getting in the habit of
running git add -A unless there’s a specific reason not to.) Then we commit
as usual:
[website (master)]$ git commit -m "Add README file"
By the way, there’s no harm in including -a via the -am combination shown in
Listing 1.5 (and despite the redundancy I often do so out of habit), so this could
just as easily read git commit -am "Add a README file". (The call to
3Atom comes with a builtin Markdown previewer, but recall from Learn Enough Text Editor to Be Dangerous
that editors such as Sublime Text often have installable Markdown Preview packages as well.
