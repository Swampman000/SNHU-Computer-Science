# CS 255 System Analysis and Design Portfolio

This repo holds two artifacts from my CS 255 work on the DriverPass project: the Business Requirements Document from Project One and the System Design Document from Project Two. Together they show the full path from gathering what the client wanted to designing a system that actually meets it.

## Project Summary
The client was DriverPass, a driver education company that runs classes, online practice tests, and on the road training. They wanted a web based system reachable from a browser, tablet, or phone so customers could reserve lessons and take DMV style practice tests, and so staff could manage reservations and packages. Big piece was secure role based access for customers, the secretary, the IT officer, and the owner, with admin controls the IT officer could use without pulling in a developer.

## What I did well
Turning a messy interview into a structured set of requirements, then carrying those straight through into the diagrams. The use case, sequence, and class diagrams all line up with the BRD instead of drifting off on their own. I do data collection software for a government job, so I think a lot about whether the next person can pick up the work after me. That carried over here. The docs are meant to be read by someone who wasn't in the room.

## One thing I'd revise
The class diagram. It's solid on attributes but light on operations. If I went back I'd add the key methods to each class so it reads more implementation ready, not just a data model. I'd also drop in a couple of error or alternate paths on the sequence diagram, since right now it only shows the happy path and real systems fail in interesting ways.

## Interpreting user needs
I started from the owner and staff interview and pulled out what they actually needed, not what sounded cool. Online reservations, practice tests, role based logins, admin controls without a developer. Those became requirements, then the requirements drove the design. This matters because the user lives in the system every day. Miss a real need and you either get expensive rework or a system nobody uses.

## How I approach design
Requirements first. Figure out who the users are and what they need before touching any structure. Then model before building. Use cases to nail down who does what, then sequence and class diagrams to work out the flow and the structure. Going forward I'd keep leaning on UML to think before I code, and I'd validate requirements with the client early instead of finding out at the end that I built the wrong thing.
