# TeamOrzo

ICS414 Summer 2018 Calendar (.ics) assignment

Your last assignment is a straightforward implementation using common software
engineering tools. This is not difficult, but requires some attention to detail. You will
work in same teams.

We will adopt the agile idea of “sprints”. You will have check-ins to make sure things
are on track and demo what you’ve accomplished during the sprint.

The task, outlined below, is to create .ics “event files”, as described in RFC 5545
https://tools.ietf.org/html/rfc5545 . Of course, you won’t be implementing
everything that’s in RFC 5545! I don’t know of any commercial implementation of
everything in RFC 5545, so you’ll be doing a small piece. Your system will generate
event files – you are not building a system to read event files. You can use an existing
calendaring system like Outlook, Google Calendar, or Mac OS Calendar to read files
(hint: that’s a good way to test the output of your system). You are building a
system to create .ics files that can be emailed or shared, and read into the recipient’s
calendars.

Most of your “deliverables” will be meeting as a team with the TA. You can meet
with the TA in person or on-line, or some combination. Your TA will help schedule
check-in times. If you miss a meeting, you don’t get any points.
The first check-in is worth 5 points. This is very simple. You will demonstrate to
the TA that:

• your team has registered your project on a project repository system (such
as github).

• everyone in the group has used a calendaring system of their choice to create
an .ics event file and then looked at the content of that file with a text editor
such (such as vim). “Reverse engineering” .ics files can offer significant
insight.

• This is also the time to ask the TA questions about the assignment.
The second check-in is worth 5 points. You will demonstrate to the TA that:

• you have functioning code that does something: You must demonstrate code,
even if it is just print statements, that generates a .ics file for a simple, single
occurrence event: Study for exam, 10am-1pm HST, 13 July 2018, in Hamilton
Library. You must then demonstrate that the calendar program of your
choice (say, google calendar) successfully reads and processes your .ics file.

• You don’t need a user interface for your first check-in since you are just
generating the .ics file for the single event described above.
The third check-in is worth 5 points. You will demonstrate to the TA that:

• you developing and performing test cases as you are developing code

• you have functioning code that does more than it did for the first check-in.
You must demonstrate a user interface for an event creation system that
uses menus and checks input for validity (i.e., no 30 February events, no
events that end before they start, …)

• you have a plan for implementing some aspects of recurring events (see
below)
The fourth check-in is worth 5 points. You will demonstrate to the TA that:
You have performed a usability test on your system with typical users. More on the
format of the usability test is to come.
The fifth and final deliverables, worth 5 points, are:

• The URL for a 5 minute video demonstration of your final project. Your demo
shall not be longer than five minutes. You can use jing.com, screencast-omatic.com, …., or if you are using a Mac, QuickTime, to capture your screen to
video. You need to demonstrate the functionality described below.

• A one-page pdf document convincing us that your system is correct. That is,
how did you test your system and what were the results?

• A link to your documented source code in your repository.

• Each team member turns in the same pdf document, same link to the
repository, and same link to the video demo.
Required functionality. You are developing a stand-alone application to create .ics
event files. You must demonstrate the following are implemented:

• Version (section 3.7.4 of RFC 5545)

• Classification (3.8.1.3). Note this is a way of users designating events as
public (default), private, or confidential.

• Geographic Position (3.8.1.6)

• Priority (3.8.1.9)

• Summary (3.8.1.12)

• DTSTART (3.8.2.4)

• DTEND (3.8.2.2)

• Time zone identifier (3.8.3.1)

• And some aspect (your choice) of recurring events (3.8.5). Recurring events
(and exceptions to recurrences) can be very complicated. Start small and do
what you can. For example, you might want to start with being able to
schedule a meeting on the 25th of every month. Then add the ability to do
exceptions, such as “except in December”).

Start small with the simplest .ics file you can generate, test, and iterate.
Everyone needs to be helpful (to other teams if necessary), patient, and not wait to
the last minute. Note that Section 4 of the RFC has several examples of .ics files and
Section 5 is Recommended Practices.

You are probably wondering why-oh-why are we doing this? It’s because an RFC
like this is a real-world specification. It’s common to be given a specification that
you don’t immediately understand, and being told to implement a subset of it. We’re
also interested in interoperability. That is, the .ics files your system creates must
work with multiple calendaring systems. Everyone has google calendar, so start
with that one.

At the end of the class you will do team peer evaluations of your team’s members,
including yourself.

If you find that you really like .ics files and calendaring, feel free to implement some
of the specifications in RFC 7986: https://tools.ietf.org/html/rfc7986

