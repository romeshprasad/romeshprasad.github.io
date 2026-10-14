---
layout: default
title: Vision
subtitle: "The research and educational program I want to build: manufacturing systems that sense, decide, act, and adapt."
permalink: /vision/
---

<blockquote class="epigraph">
  “The machine does not isolate man from the great problems of nature but plunges him more deeply into them.”
  <cite>Antoine de Saint-Exupéry, <em>Wind, Sand and Stars</em></cite>
</blockquote>

## Why this matters

As machines become more intelligent, they change not only what can be automated but also what
people are asked to do. Greater autonomy can reduce the need for direct human control, yet it can
also add new layers of coordination, supervision, and decision-making. I believe the goal of
intelligent technology should not be autonomy for its own sake. Intelligent systems should take on
more of the operational complexity of coordinating, controlling, and adapting machines, so that
people can focus on the problems that require human judgment, creativity, and expertise.

Modern manufacturing makes this challenge especially visible. **A factory may contain intelligent
machines without being an intelligent factory.** Robots, machine tools, sensors, material-handling
systems, and decision algorithms may each be highly capable, yet integrating them into coordinated,
adaptive system behavior remains difficult, especially when equipment is heterogeneous, conditions
change, and decisions must be made in real time.

<div class="question question-inline">
  <blockquote>
    How do we make manufacturing systems capable of turning intelligence into physical action,
    reliably, adaptively, and across heterogeneous equipment?
  </blockquote>
</div>

## Four connected capabilities

<div class="vision-loop">
{% include loop.html %}
<div>
{% for area in site.data.research %}
<p><a href="{{ '/research/' | relative_url }}#{{ area.id }}"><strong>{{ area.verb }}.</strong></a> {{ area.question }}</p>
{% endfor %}
</div>
</div>

The scientific challenge is not simply to improve each capability on its own. It is to understand
how they interact well enough that **intelligence emerges at the level of the manufacturing system**,
rather than staying confined to individual algorithms and machines.

## How I arrived here

I came to this question by repeatedly running into the gap between what an intelligent algorithm
can decide and what a physical manufacturing system can actually do.

During my **Ph.D. at Syracuse University**, I studied autonomous recovery from disruptions in
cyber-manufacturing systems. That work taught me that recovery requires more than generating a new
decision. A system must recognize that its state has changed, choose a response, execute it on
physical equipment, and evaluate what happens next.

My **postdoctoral research at the University of Rhode Island** broadened this from recovery to
system-level coordination: how shared resources should be scheduled, how computational decisions
are executed on physical robots, and how heterogeneous equipment can take part in the same
intelligent system. Each problem exposed another part of the same challenge. Intelligence at the
level of a single algorithm or machine is not enough.

## The program I want to build

**In the near term**, I will develop three foundations:

<div class="pillars">
  <div><h3>Decision methods</h3><p>Characterize how the structure of manufacturing decision problems determines which computational approaches (reinforcement learning, optimization, metaheuristics) are appropriate.</p></div>
  <div><h3>Execution architectures</h3><p>Develop capability representations and architectures that let decisions move across heterogeneous physical equipment.</p></div>
  <div><h3>State awareness</h3><p>Study how multimodal information can give systems the awareness they need to change decisions as conditions evolve.</p></div>
</div>

**Over a longer horizon, these directions converge.** I envision a manufacturing system that
recognizes a disruption or a new production requirement, determines the nature of the decision
problem it faces, selects or combines the right computational tools, translates its response into
coordinated actions across available equipment, observes the consequences, and adapts again.

The purpose is not to eliminate human involvement. It is to move people away from continuously
managing low-level operational complexity and toward **defining objectives, setting constraints,
supervising behavior, interpreting the unexpected, and making the engineering judgments** for which
human expertise remains essential.

## A lab that is also a classroom

I want my laboratory to serve as both a research environment and an educational one. The physical
systems used to investigate research questions can also become the platforms through which
students learn manufacturing, automation, robotics, sensing, optimization, and AI.

<div class="pillars">
  <div><h3>Multi-robot system</h3><p>Research in autonomous coordination; students learn robotics, material handling, and systems integration.</p></div>
  <div><h3>Instrumented CNC machine</h3><p>Research in intelligent process monitoring; students connect manufacturing processes with sensing and machine learning.</p></div>
  <div><h3>Heterogeneous testbed</h3><p>Research in vendor-agnostic control; students face the real challenges of integrating industrial equipment.</p></div>
</div>

Real manufacturing systems rarely behave like textbook problems. Constraints appear that nobody
anticipated, sensors misbehave, and algorithms that work in simulation fail when deployed. I want
students to meet these realities, because learning to respond to them is part of becoming an engineer.

As an advisor, I want to do more than hand out problems. I want to teach students to **find worthwhile
problems themselves**: to move from observing a limitation in a physical system, to formulating a
research question, to choosing or developing a method, to evaluating it critically, and to seeing
what new questions the result opens up.

<p class="closing">
  As machines become more intelligent, people should not become more distant from difficult
  engineering problems. Technology should change the level at which we engage with them.
  My goal as a researcher and educator is to make that transition possible.
</p>
