---
title: Get started
permalink: /get-started/index.html
description: 'How do you implement get started with common guide for your organisation?'
layout: page
---

## Build Your Own Handbook

This project is free and easy for any community group to set up and use their own copy.

It can be implemented in four managable chunks, separated by their skill area. Please note that implementation requires a basic understanding of the Git Version Control System and basic web server hosting.

If you're not familiar with these concepts, feel free to [contact us]() for implementation support options

```
! commonguide is CC-SA, you must maintain this license when making a copy !
```

### 1. Find.
Read through some curations, and build your idea on what curation you'd like to adopt, or start with.

Here are the curations managed by Common.Guide:


 - [Main](https://github.com/CommonGuide/commonguide/)


Community curations will be here eventually also

{% set itemList = collections.allPosts %}
					{% asyncEach item in itemList.slice(2, 4) %}
            {% set headingLevel = "h3" %}
						{% include "partials/card-blog.njk" %}
					{% endeach %}

### 2. Fold. 
Bring a proposal for implementation to your group!

2.1 Introduce common.guide and the curation you think fits the best!
It might be useful to explain the benefits of publicly hosting your policies and sharing their innovations with other groups.

2.2 Run through the policies, highlight core components that you'd need to alter
Take your time to outline how the curation would impact the current operations your group are undertaking. Where policies already exist in both your organisation and the curation you've chosen, what will happen? (will the policies merge, will one take precedence and be improved by innovations of the other?)

2.3 Resolve through consensus or whatever decision making structure your group uses.
Get the "yes" you need to go ahead with implementation.

### 3. Fork.
Make a copy of your curation of choice

Follow the instructions on the curations repository to fork it to you own account.

2.3 Revise the curation
Once you've established a clear interest from your group

Adjust the variables in the .env file. These values will get populated throughout the documents and allow you to save time by not needing to copy and paste them in everywhere.
#### 3.1 Setup your own handbook.yourwebsite
It basically takes your policies and turns them into a neat web page that's easy to digest. See our [demo](https://demo.common.guide).

The project runs on a software called [MKDocs](https://www.mkdocs.org/). You can follow their hosting instructions [here](https://www.mkdocs.org/user-guide/deploying-your-docs/)

You will benefit from using some level of automation in your deployment. This will mean that when you update the policies and attributed to the curation repository it automatically pushes those changes to handbook.yourwebsite!

In order to point the project to your own web domain, you will need to follow the hosting steps linked above. You will also need to configure the DNS for your site as per the mechanisms your registrar provides. If you're struggling to complete this step, [contact us for implementation support]()

### 4. Ferment. 
Run the policy and iterate!

Let your group run as normal and learn from what works well and what doesn't!

If you think that your improvement would benefit others, please make a pull request to the curation you forked from!

#### 4.1 Sign up to the Loomio forum

Still to be set up!

#### 4.2 Publishing your curation
Make your own Curation available for people to iterate on! Share your work, pull request things you think would benefit upstream!

For now, just have your fork on your git platform of choice. Later on we'll have a way to display them!

<!-- loop docs -->
{% set headingLevel = "h2" %}

{% css "local" %}
  {% include "css/custom-card.css" %}
{% endcss %}
