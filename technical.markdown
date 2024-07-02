---
layout: page
title: Technical
permalink: /technical/
---

# South Park Commons # 

In the 0-1 program, I ran experiments with open-source and commerical LLMs and designed a second brain for physicians to accelerate knowledge building in academic hospitals. 

In a canonical clinical database, physicians spend 1-4 hrs/day reading patient notes before and after visits, and up to 8 minutes answering natural language questions. These factors decrease clinical diagnostic and prognostic accuracy at the point-of-care and increase clinical burnout. Motivated by my own priors from medical school, I worked to develop a LLM-based patient control dashboard that empowered physicians with natural language queries, the parsing of unstructured medical notes into structured ouputs, data visualizations, and intelligent analysis of user actions.

- Tested performance of 15 open-source clinically fine-tuned modelsagainst commercial LLMs on question-answering
- Designed a platform to turn unstructured clinical notes into structured outputs
- Developed orchestration tools for LLM queries  

I established partnerships with 500+ bed hospitals, joined the Artificial Board of AI in Medicine, met with 100+ physicians and researchers, wrote product roadmaps and engineering designs, and coded daily.

# Cash App #

I worked on the core product platform team to accelerate the velocity of product developers for 2 years. I thought about:

- how to manage and prevent high severity incidents 
- tradeoffs between consistency and availability in mobile banking
- how to engineer robust models of user trust 
- systems to unblock engineers faster
- the composition of scalable organizations and technical systems

I worked primarily on distributed systems problems, spent 30% of my week explaining technical architecture to other engineers, and contributed to open source projects. Below is a sampling of projects:

<details>
<p><summary><strong>Mobile Deploys</strong></summary></p>

Q: How do you empower mobile engineers with controls (canary rollouts, automated rollbacks, autodeploys) to deploy the latest release from a monorepo to app users?  

A: Worked on a team of 2 over 2 months to build a service that uploaded mobile releases to the CDN, autodeployed these releases incrementally, published actions taken to mobile engineers via chatops, and triggered automated rollbacks. This started to turn a manual Q/A release process led by non-engineers into an automated one. Also enabled high-velocity deploys (daily instead of 1-3 weeks). Java/Kotlin, PostgreSQL, Cloudflare CDN, Github APIs, LaunchDarkly, PagerDuty, Slack APIs, Cron. 
</details>

<details>
<p><summary><strong>State Machines</strong></summary></p>

Q: How do you migrate a server-side state machine to be client-side and create a new model of trust? 

A: In an effort to reduce latency, improve UX, and fork the presentation and domain layers, I worked on a team of 4 to start migrating user data that shuttled through a server-side state machine to client-side control. I worked fullstack and rewrote domain APIs, frontend UIs, and build a JWT-based authorization system to enable a client-server trust model. We reduced latency in app onboarding, enabled users to flexibly navigate between screens, and empowered engineers to build a user experience in 1-3 weeks instead of 1-3 months. Java/Kotlin, gRPC/Protobufs, Jetpack Compose, Google Tink Cryptographic Library. 
</details>

<details>
<p><summary><strong>Internationalization</strong></summary></p>

Q: How do you architect an internationalization system responsible for translating English copy so that existing microservices will not encounter failures?

A: Built a library that versioned and diffed all uploaded app copy in the document store to enable services to successfully rollback and forward and fetch modified app copy. This project unblocked the internationalization efforts so engineers could continue to deploy their services in parallel with app copy being translated by the internationalization services. Java/Kotlin, gRPC/Protobufs, AWS S3. 
</details>

<details>
<p><summary><strong>Rate Limiting</strong></summary></p>

Q: How do you prevent degrading microservices from crashing the central router responsible for shuttling user data to and from the app? 

A: Extended existing rate limiting libraries and implemented this feature in the central routing microservice owned by my team to throttle traffic from degrading services and prevent total system failure. Java/Kotlin, LaunchDarkly, microservice library frameworks.

</details>
