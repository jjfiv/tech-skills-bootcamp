# Tech Skills Bootcamp

## Before you start

If you do not have access to a linux system, we strongly recommend using [Vagrant](https://www.vagrantup.com/) in conjunction with [VirtualBox](https://www.virtualbox.org/). 

Note that if you're on Ubuntu Linux already and you want to try this Vagrant thing out, you're going to want to get the on from the website and not the one from ``apt-get``, as it is [out of date and not compatible with most images](https://github.com/fideloper/Vaprobash/issues/322).

## Fork this repository!

Fork this repository, and clone your copy once you're inside vagrant.

    https://github.com/${GITHUB_USER_NAME}/tech-skills-bootcamp.git 
    cd tech-skills-bootcamp # go inside
    git remote add upstream https://github.com/CSWomenUMass/tech-skills-bootcamp.git # tell git that it came from a fork!

## Add your username to the participants file!

Open the file for editing with ``nano``. If you're familiar with ``vim`` or ``emacs`` we've installed those for you, too. ``nano`` is very simple to use, though.

Add your CS or github username to the file; go ahead and make one up if you don't have one -- and don't delete anyone elses! Feel free to also record the date!

    nano participants.md

Tell ``git``, the version control system that you've changed the file, and that you're done making changes for this commit:

    git add participants.md
    git commit # save changes locally

At this point, git may complain that you haven't configured it -- within vagrant, that is:

    *** Please tell me who you are.

    Run

      git config --global user.email "you@example.com"
      git config --global user.name "Your Name"

    Now tell ``git`` you're done changing things for now, and push your changes up to your fork of the repository.

One of the best features of `git` is that it tries to walk you through why it is confused and how to fix it. That doesn't mean it always explains things very good, so ask if you get stuck.

If ``git`` doesn't complain, it will pop open ``nano`` and ask you to write a message describing your changes. Mine was ``This is so much fun :)``.

    git push # send them up to the server
    git pull upstream master # pull any changes from upstream CSWomenUMass/tech-skills-bootcamp

At this point, you may have to merge other people's changes. If you get stuck, ask for help! ``git`` attempts to walk you through the process, but sometimes this can get complicated, if it thinks you edited the same line as other people.

    git push # if you merged

Now, submit your changes as a pull request on github. One of the instructors will accept your pull request, and you'll likely get an email notification about it.

## Congratulations!

You're done for now. Some UNIX/bash review slides are coming soon, so there'll be more refresher material to work through.

Here's a challenge: Write a unix command to print out the number of participants in that file. A good starting point is ``wc -l`` which will count the number of lines in the file, but that will include the title as well! Maybe ``grep`` can help. Recall that google and stackoverflow can be a good reference, but so is ``man grep``.

