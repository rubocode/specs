> [home](../)

![banner](/specs/photos/banner.png)

## Introduction

I was first introduced to Software Requirements Specifications (SRS) in
practical terms once I joined the Finance Dest Trading System Team (FDTS)
at Salomon Brothers as a Programmer Analyst.
Salomon Brothers was my first employment after graduation in 1996.
I had a few years of programming experience under my belt already.

Programmers often take SRS documents as something out of their scope to create.
As I matured as a programmer, it became quite clear that one of the most significant
problems of practical software development was that folks didn't quite yet know
how to specify software in a pragmatic and durable fashion.

In 2017, I joined the Sri Lanka Institute of Information Technology (SLIIT)
as a Product Architect to attempt to rescue its Student Information Management System
(SIMS) project.  There was no SRS or even a way to capture any domain knowledge.
They had been working in a somewhat agile fashion, considering working software as
the priority, but — in the end winging it.

When I joined, the Project Manager — who was also the Head of the Software Engineering
Services Division (SESD) — had been working on it for more than a decade.
They had evolved from a Microsoft Access project into a Microsoft SQL Server project
using C#.  All the domain knowledge was inside two brains — that of the Project Manager
and the Technical Lead. The project was dragging on endlessly.

The project was ridden with internal politics and I left after my initial six month
contract.  But, the silver lining was that I began to explore requirements
capture techniques and methodologies with great zeal.
While I was still working at SESD, I came across the book
_Rapid Agile Business System Analysis: Fast, Agile, Measurable Results
(Frantzen, Trond: 2015)_.
The idea of _events_ being central to requirements gathering took root in me
at that time.

The most fundamental idea in computing is one of input, process and output.
Any entity can be thought of as a processor.
It can also be viewed from an anthropomorphic perspective.
Why not consider each entity as an agent that responds to stimuli.
Then we can explore the behaviroal aspects of the agent as a stimulus response
organism — a la B.F. Skinner (Behavioral Psychologist).

It helps to remember the seminal definition of Artificial Intelligence put forth by
Alan Turing.  If you can't distinguish between the agent and a human — both of them
placed in a black box scenario — based on input and output (stimulus and response),
the agent is considered intelligent.

Now, we can look at any black box system as a Stimulus Response System (SRS &#x1F609;).
Let's begin calling the stimuli by another name — triggers — an we are in business
with events.  An event encapsulates a trigger and a response togther into a
convenient abstraction.

> An event describes a trigger with a response to that trigger.
> The response may also invoke other triggers in turn.
> The event is complete when no more triggers are invoked by the response.

Suppose we — as in the good old days — slide a quarter into a vending machine
(VM &#x1F609;) and pull a crank and get a can of Coke&trade; out.
Let's assume that the only product dispensed by the VM is Coke&trade;.

![photo](photos/tar.png)

* The trigger is the pull of the crank.
* The VM responds by spitting out a can of Coke&trade; and ringing a bell.
* The intelligence inside the VM is an agent.
* It gets triggerred by the pull on the crank.
* The agent then triggers the dispenser to spit out a can of Coke&trade;
* It also triggers the bell to ring!

> An _event_ captures the _response_ of an _agent_ to a _trigger_.
> A response, in turn, is another set of events.
> An event is complete when its response cluster doesn't generate any more triggers.

We can now capture a useful acronym to to summarize what an event is:

> An EVENT is a tuple: Trigger, Agent, Response (TAR).

Now, we are in business.  We have the essence of a sort of fractal — a pattern that
repeats itself however deep you go.  We can capture any action inside the system
as an EVENT.

* A button press is an event.
* A customer order is an event.
* A customer payment is an event.
* A product shipment is an event.
* A use case is an event.
* A function call is also an event!
* A clock cycle is an event!

How cool is that!

> It's turtles all the way down!

PS: If you're curious as to what happened to the SIMS at SLIIT, let me be brief.
They outsourced the project to a reputed local company for multiple millions.
After about 3 years, they abandoned the project.
Then they went into a venture with an Indian company to modify an already
existing SIMS app to suit their needs.
After about 4 years and wasting yet multiple millions, that also folded.
Now — in 2025 — they are kind of back at square one.
Ahem, actually worse:  they have hired an outside development team and running
the project themselves.

> If they only bothered to capture what they needed to build and had a decent
> high-level view!

Here, I am offering hope!
