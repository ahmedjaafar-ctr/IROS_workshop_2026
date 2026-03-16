---
title: Home
---

# Bridging the Gap between Neural and Symbolic World Models for Robot Planning, Reasoning, and Action

{% include figure.html img="workshop_banner.png" alt="banner image here" caption="" width="75%" %}


## Abstract
World models have emerged as a central paradigm in robot learning, planning, and reasoning, yet the term spans different meanings across communities: high-dimensional neural dynamics models that predict future latent states (e.g., DreamerV3 [1]), symbolic transition systems such as PDDL-style domain models [2], task-level abstractions, and simulators. Despite momentum around neural world modeling and policy-centric approaches, such as Vision-Language-Action models [3], comparatively little attention has been paid to the structure, representations, and limitations of world models that govern state evolution and long-horizon reasoning. Recent world model focused [4–10], and adjacent [11–21] workshops, including at IROS 2024–2025 [17–21], have emphasized neural approaches or the use of neural methods (e.g. Vision-Language-Models) to induce symbolic models. In contrast, this workshop focuses on the intersection between neural and symbolic world models as complementary paradigms, along with neuro-symbolic approaches, for robot planning and decision-making.
We aim to bring researchers across neural, symbolic, and hybrid communities to clarify terminology, align assumptions, identify shared challenges, etc. Furthermore, the workshop intends to highlight hybrid world modeling frameworks that integrate learned latent dynamics with structured symbolic abstractions, ideally enabling improved data efficiency, generalization, interpretability, uncertainty estimation, long-horizon reasoning, etc. Emphasis will be placed on manufacturing-related domains—such as precision assembly, occluded bin-picking, production reconfiguration, and inspection—where structured task knowledge and state prediction under uncertainty are critical. By positioning world models as explicit components of robotic systems, alongside planning and policy learning, this workshop seeks to articulate new principles for hybrid world modeling in robotics.

## Objectives
* What constitutes a “world model” in robotics, and how can neural and symbolic perspectives be formally related or unified?
* How do world models differ in terms of their horizon limit and coarseness level? How can different types of world models interact with each other?
* How can neural and symbolic world models be formally unified, and what principled methods enable bidirectional translation between neural representations and symbolic abstractions (neural→symbolic and symbolic→neural), forming “neuro-symbolic” methods?
* What hybrid architectures (e.g., latent dynamics + symbolic constraint module, neuro-symbolic graph networks, neuro-symbolic program induction) are most effective across robotics tasks?
* How can symbols or predicates be extracted, grounded, and updated from high-dimensional latent world models, and what algorithms enable translation from latent neural states to human-interpretable symbolic representations?
* Conversely, how can symbolic knowledge and priors (rules, PDDL, knowledge graphs) be compiled into inductive biases, constraints, or architectures for neural world models?
* How can symbolic predicates, abstractions, and priors (e.g., PDDL, knowledge graphs) enhance neural world models’ state prediction, long-horizon reasoning, uncertainty estimation, data efficiency, and cross-task generalization?
* How can symbolic planners be integrated into neural world models for trajectory generation, data collection, and safe exploration?
* How does abstraction and task-relevance affect the need for fidelity of symbolic and neural world models?
* How do artificial neural and symbolic world models compare to biological models found in humans and animals?
* What does it mean for a world model to be good enough? Ex: task success, modeling fidelity, to be composable, etc?
* What benchmarks, metrics, and manufacturing-relevant tasks best evaluate hybrid world models in terms of scalability, interpretability, and deployment readiness?


## Speakers

<div class="people-grid-container">
  {% for person in site.data.speakers %}
    <div class="person">
      <div class="circle-crop-wrapper">
        <img src="{{ person.image | relative_url }}" alt="{{ person.name }}"
          {% if person.position %}
            style="object-position: {{ person.position }};"
          {% endif %}>
      </div>
      <h3>{{ person.name }}</h3>
      <p>{{ person.role }}</p>
      <p>{{ person.affiliation }}</p>
    </div>
  {% endfor %}
</div>