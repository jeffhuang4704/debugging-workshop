
## Gophercon 2020 Debugging Workshop

To get back to here: [bit.ly/debugging-workshop][bitly]  
Slack Channel: [#gophercon-2020-debugging-workshop][slack]


### Course Objective

Solving bugs can be incredibly challenging. It can often feel like our
programs have the upper hand. My goal for this course is to instill in you
the confidence that you can understand and squash your bugs, no matter how
challenging they are.

The next time you encounter a difficult bug, I'd like for you to be able to
say:

> I don't know what is wrong with my program but I know how to find out!

In this course, we will be covering a number of tools that I have found
useful in understanding Go programs.

### Before Starting

You will need to clone this repo:

```
git clone https://github.com/jasonkeene/debugging-workshop
```

There are a few things you should have setup on your machine before starting
on the exercises. You will need to:

- [Install Go][install-go]
- [Install Delve][install-delve]
- [Install Docker][install-docker]

A Linux machine will be needed for the more advanced exercises as they
utilize capabilities specific to Linux. If you do not have a Linux machine
handy, no worries. This repo contains a `Vagrantfile` that will provision a
Linux VM for you. It is recommended to do this in advance of the workshop as
it can take some time to download the machine image and provision the VM. You
will need to:

- [Install VirtualBox][install-virtualbox]
- [Install Vagrant][install-vagrant]
- Run `vagrant up` from the repo root to provision the VM
- Get a shell on the VM by running `vagrant ssh`

If you are not using the Vagrant VM you will need to:

- [Install rr][install-rr]
- [Install bpftrace][install-bpftrace]

You can see how these were installed in the VM by looking at the
`vagrant-provision.sh` file.

### Exercises

This workshop is broken down into a series of exercises. We will go through
these individually during the class:

- [Introduction][00]
- [Starting a Debugging Session][01]
- [Navigating Your Program][02]
- [Demystifying Debuggers][03]
- [Remote Debugging][04]
- [Debugging Inside a Container][05]
- [Debugging from Core Dumps][06]
- [Automating Delve][07]
- [Deterministic Debugging][08]
- [pprof][09]
- [bpftrace][10]

Please ask questions as we work through these exercises! If I went too fast
over something that needs additional explanation please stop me. Some of the
later sections build on earlier sections so it is important that we all
understand the material before moving forward. You can also ask questions
during the breaks if you prefer.

### Instructors

<div>

<img src="./jason-keene.jpg" width="130" height="130" align="left" />

#### Jason Keene

Instructor - Delve User

Contact: [Slack](https://gophers.slack.com/archives/D1KEZBKD0)

<br clear="left" />

</div>

<div>

<img src="./derek-parker.jpg" width="130" height="130" align="left" />

#### Derek Parker

Instructor - Creator of Delve

Contact: [Slack](https://gophers.slack.com/archives/DQU4ZQW3E)

<br clear="left" />

</div>

<div>

<img src="./warren-fernandes.jpg" width="130" height="130" align="left" />

#### Warren Fernandes

TA

Contact: [Slack](https://gophers.slack.com/archives/DCKBZL41K)

<br clear="left" />

</div>

### Feedback

If you have any feedback about this workshop, the presenters, the content,
the remote format, etc please let us know by filling out [this form][feedback]!

[bitly]: https://bit.ly/debugging-workshop
[slack]: https://gophers.slack.com/archives/C01BJJMDMB9

[install-go]: http://golang.org/dl
[install-delve]: https://github.com/go-delve/delve/tree/master/Documentation/installation
[install-docker]: https://docs.docker.com/desktop/
[install-virtualbox]: https://www.virtualbox.org/wiki/Downloads
[install-vagrant]: https://www.vagrantup.com/downloads
[install-rr]: https://rr-project.org/
[install-bpftrace]: https://github.com/iovisor/bpftrace/blob/master/INSTALL.md

[00]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/00-introduction
[01]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/01-starting-a-debugging-session
[02]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/02-navigating-your-program
[03]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/03-demystifying-debuggers
[04]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/04-remote-debugging
[05]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/05-debugging-inside-a-container
[06]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/06-debugging-from-core-dumps
[07]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/07-automating-delve
[08]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/08-deterministic-debugging
[09]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/09-pprof
[10]: https://github.com/jeffhuang4704/debugging-workshop/tree/master/exercises/10-bpftrace

[feedback]: https://forms.gle/7utCyAqPwMcPBdQJ9
