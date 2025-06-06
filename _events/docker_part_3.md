---
layout: page
title: "Introduction to Docker, Part 3"
event_date: "TBD"
start_time: "TBD"
end_time: "TBD"
location: "University of Geneva, Room TBD"
speakers:
  - name: "Carson Sprock"
    title: "Data Scientist"
    bio: "Carson is a data scientist from California who has worked in the freight and commodities industries. He is a generalist but has a special interest in time series."
    url: "https://csprock.github.io"
# agenda:
#   - time: "6:00 PM - 6:45 PM"
#     activity: "Presentation and Q&A"
#   - time: "6:45 PM - 8:00 PM"
contact_email: "contact@genevalytics.ch"
presentation_url: https://github.com/csprock/docker_tutorials
upcoming: true
hide: false
series_number: 6
---

The final presentation of the Docker series introduces container orchestration and brings together all the learnings from the previous lessons to build a self-contained dockerized application featuring a database and user-interface to browse it.

### Event Details

- **Date:** {{ page.event_date | date: "%B %d, %Y" }}
- **Time:** {{ page.start_time }} - {{ page.end_time }}
- **Location:** {{ page.location }}
{% if page.presentation_url %}- **[Presentation Material]({{ page.presentation_url }})** {% endif %}

### Speakers

{% for speaker in page.speakers %}
**[{{ speaker.name }}]({{ speaker.url }})**
*{{ speaker.title }}*

{% if speaker.bio %} {{ speaker.bio }} {% endif %}


{% endfor %}

### Agenda

{% for item in page.agenda %}
1. **{{ item.time }}:** {{ item.activity }}
{% endfor %}

---

For any questions about this event, please contact us at [{{ page.contact_email }}](mailto:{{ page.contact_email }}).