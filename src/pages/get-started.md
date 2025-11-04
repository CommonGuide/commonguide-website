---
title: Get started
permalink: /get-started/index.html
description: 'How do you implement get started with common guide for your organisation?'
layout: page
---

## Build Your Own Handbook

This project is free and easy for any community group to set up and use their own copy.

Contact us for implementation support options

```
! commonguide is CC-SA, you must maintain this license when making a copy !
```

### 1. Find. Pick out the closest curation for your use case
Here are the curations managed by Common Guide:
{% set itemList = collections.allPosts %}
					{% asyncEach item in itemList.slice(0, 2) %}
            {% set headingLevel = "h3" %}
						{% include "partials/card-blog.njk" %}
					{% endeach %}
Here are where you can find community curations:
{% set itemList = collections.allPosts %}
					{% asyncEach item in itemList.slice(2, 4) %}
            {% set headingLevel = "h3" %}
						{% include "partials/card-blog.njk" %}
					{% endeach %}

### 2. Fold. Bring the proposal for implementation to your group

2.1 Introduce common.guide and the curation you think fits the best!

2.2 Run through the policies, highlight core components that you'd need to alter

2.3 Revise the curation

Adjust the variables in the .env file. These values will get populated throughout the documents and allow you to save time by not needing to copy and paste them in everywhere.

2.4 Resolve through consensus or whatever decision making structure your group uses.

### 3. Fork. your curation of choice

Follow the instructions on the curations repository to fork it to you own account.

#### 3.1 Setup your own handbook.\*domain\*

It basically takes your policies and turns them into a neat web page that's easy to digest. See our [demo](https://demo.common.guide).

The project runs on a software called [MKDocs](https://www.mkdocs.org/). You can follow their hosting instructions [here](https://www.mkdocs.org/user-guide/deploying-your-docs/)

In order to point the project to your own web domain will depend on your own registrar but broadly speaking it's the same as pointing a domain to any other service.

### 4. Ferment. Run the policy and iterate!

Let your group run as normal and learn from

#### 4.1 Sign up to the Loomio forum

#### 4.2 Publishing your curation
Make your own Curation available for people to iterate on! Share your work, pull request things you think would benefit upstream!

<!-- loop docs -->
{% set headingLevel = "h2" %}

{% css "local" %}
  {% include "css/custom-card.css" %}
{% endcss %}
