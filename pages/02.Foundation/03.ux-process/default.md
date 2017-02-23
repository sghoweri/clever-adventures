---
title: 'UX Process'
---

{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    classes: "c-heading--xxlarge",
    text: "UX Process"
  }
} %}
The work of the Pegasystems Digital UX team serves the people who buy, sell and build with our products. Our user-centered design process is guided by three key principles:
- **Understand the design problem.** Prior to beginning new work, we assess the goals of a project, identify gaps in our knowledge, and conduct research to fill in those gaps.
- **Prototype, validate and iterate rapidly.** We work directly with developers, stakeholders and end users to create and test potential solutions to the design problem.
- **Measure and continuously refine.** As work is launched, we keep track of key metrics via usability testing and analytics, and identify areas that can be improved.

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "The 5-Step process"
  }
} %}

Our 5-step UX process helps maintain the consistency and quality of our work while supporting a Lean/Agile development process.

{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "Create the design brief"
  }
} %}

All projects start with a kickoff meeting between a UX lead and a technical lead. In this meeting, we start by establishing the key business goals related to the design problem, as well as any technical or business constraints that may exist. We also establish key personas to guide the design process, and we document key scenarios the design is meant to accommodate using <a href="https://jtbd.info/replacing-the-user-story-with-the-job-story-af7cdee10c27?gi=f40ebfb5ca7d#.7rkwmcgy4">job stories</a>.

Within a week of the kickoff meeting, the goals, constraints, personas and scenarios are combined into a <a href="https://articles.uie.com/short_form_creative_brief/">short design brief</a>, along with a set of proposed milestones and deliverables for the project. This brief serves as our touchstone throughout the design process.

{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "Conduct research"
  }
} %}

While completing the design brief, the UX lead consults with the team to determine what types of research are needed to flesh out our understanding of the problem space. Types of research we conduct may include:
- **Rapid usability testing** of features being redesigned, to identify issues with current functionality;
- **Analytics or heatmap data** to understand broad usage patterns;
- **<a href="https://en.m.wikipedia.org/wiki/Tree_testing">Tree tests</a> or <a href="https://en.m.wikipedia.org/wiki/Card_sorting">card sorting</a>** to test information architecture or navigation;
- **User interviews or <a href="https://hbr.org/2009/03/ethnographic-research-a-key-to-strategy">ethnography</a>** to gain insight into user populations unfamiliar to the UX team;
- **UI pattern and interaction design research** to identify best practices and potential enhancements to our UI patterns.

{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "Ideate and prototype"
  }
} %}

As we begin to explore the problem space, we sketch, generate ideas, capture feedback from technical and business stakeholders, and start to build out prototypes of the most successful design solutions.

We use <a href="http://www.axure.com/">Axure</a> to create responsive, mobile-first prototypes that mimic real interactive behavior. These prototypes can be sent to stakeholders for review, displayed in meetings, and used for online usability testing, to validate designs prior to development.

When work is ready for development, we annotate our prototypes extensively to help developers understand how functionality is expected to behave, and which design patterns they can reference. We also create templates inside of <a href="http://vpatternlab/">Pattern Lab</a> to reference HTML and Sass code.

{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "Guide development"
  }
} %}

As work goes into development, we work alongside developers to identify scenarios that were missed during the design process, answer questions that come up, and ensure that the look and feel of the finished product aligns with our design standards.

{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "Measure and iterate"
  }
} %}

Post-launch, we work with stakeholders to identify and prioritize future enhancements, and we conduct UX research to validate the new features and uncover additional improvements to be made. We may also track key analytics related to the new feature, to determine if broad usage patterns are in line with expectations.
