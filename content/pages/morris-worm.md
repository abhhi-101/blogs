Title: Morris worm
Date: 2022-4-12 10:20
Tags: hacking stories, Morris worm
Category: stories
Slug: morris-worm
Authors: Abhishek Birdawade
Summary: Morris worm

> Worms everywhere
>>  -- by unpatched system

![Morris](../images/morris.jpg)

The Morris Worm was a self-replicating computer program (worm) written by Robert Tappan Morris. He was a student at Cornell University. He released the computer worm from one of the MIT’s computer on *November 2, 1988*.

According to Morris, the purpose of the worm was to gauge the size of the precursor “Internet” of the time – ARPANET – although it unintentionally caused denial-of-service (DoS) for around 10% of the 60,000 machines connected to ARPANET in 1988.
The worm spread by exploiting vulnerabilities in UNIX send mail, finger, and rsh/rexec as well as by guessing weak passwords. Yes, Unix was vulnerable too.

### How it worked?

Before spreading to a new machine, the Morris Worm checked if the machine had already been infected and was running a Morris Worm process. If a target machine had already been infected, the Morris Worm would re-infect it 1 in 7 times. This practice of “1-in-7 re-infection” ensured that a user could not completely avoid a Morris Worm infection by creating a fake Morris Worm process to pretend his or her machine was already infected. It also, caused some users’ machines to be infected many times – once too many Morris Worm processes were running on a target machine it would run out of computing resources and begin to malfunction.

The United States vs Morris (1991) court case resulted in the first conviction under the 1986 Computer Fraud and Abuse Act, with Morris receiving a sentence of three years in prison, 400 hours of community service and a $10,000 fine. It was easy back then.

The floppy containing Source code of the Morris Worm is kept in a Computer History Museum, what an achievement, isn’t it?

![floppy with virus](../images/source.webp)

That’s it for today, see you in the next blog, till that have a good day and babye!!

--- 

&copy; hackkeencyber