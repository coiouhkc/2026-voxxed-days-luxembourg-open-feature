---
marp: true
title: OpenFeature -- one flag to rule them all
theme: uncover
paginate: true
_paginate: false
header: ![image](images/OpenValue-Wordmark-TT-Blue.png)
style: |
    :root {
        font-family: 'Montserrat', 'Avenir Next';
        color: #1d252d;
        --color-background: #f1f5f6;
        --color-background-code: #cbd9da;
        --color-background-paginate: #cbd9da;
        --color-foreground: #345;
        --color-highlight: #809fa2;
        --color-highlight-hover: #014046;
        --color-highlight-heading: #99c;
        --color-header: ##1d252d;
        --color-header-shadow: transparent;
    }

    section {
    }

    header {
        display: flex;
        justify-content: flex-end;
        height: 32px;
    }



---

### OpenFeature

###### one flag to rule them all

---

### What are feature flags?

Way to change the system behaviour at runtime without hassle.

---

### What are feature flags (contd.)?

Software development technique that allows enabling, disabling or changing the behaviour of certain features or code paths in a product or a service at runtime, without modifying the source code or re-deployment/service interruption <a href="#footnote-1">[1]</a><a href="#footnote-2">[2]</a>.

<h4></h4>
<sub><sub><sub><ol>
    <li id="footnote-1">https://www.dynatrace.com/news/blog/feature-flags-with-openfeature-and-dynatrace/</li>
    <li id="footnote-1">https://www.youtube.com/watch?v=euYhIn4leW0</li>
</ol></sub></sub></sub>

---

![bg 70%](images/meme.png)

---

### What are feature flags (contd.)?

###### Toggles → boolean-only?

No! Whoever refactored a nested `if/then/else` to a `switch` knows it.

---

### Why feature flags (contd.)?

* maintenance switch
* kill switch (data processing)
* feature paywall
* country-specific legislation
* A/B testing

---

### Why feature flags (contd.)?

###### 12factor + K8s?

* no K8s
* no DevOps
* heterogenous landscape
* rare maintenance windows
* etc.

---

### How feature flags?

###### Demo!

Pizza store

---

### How feature flags (contd.)?

###### Caveat scriptor codicis

* amount
* stale flags
* obsolete/ outdated comments/ documentation
* combinatorial explosion of testing effort
* feature flag inter-dependencies

---

![bg left](images/qr.png)

# Q&A