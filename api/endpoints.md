---
description: >-
  Wir nutzen für unsere öffentliche API eine REST API. Hier findest du eine
  Liste aller Endpoints die öffentlich verfügbar sind.
---

# 📍 Endpoints

{% swagger method="get" path="/users" baseUrl="https://api.thedannicraft.de/data/discord/gamerforge" summary="" %}
{% swagger-description %}
Rufe Daten zu den öffentlichen User-Daten ab.
{% endswagger-description %}

{% swagger-response status="200: OK" description="ERFOLG" %}
```javascript
{
    "members":601, // Insgesammte User(mit Bots)
    "bots":21, // Anzahl der Bots
    "users":580, // Anzahl User(ohne Bots)
    "online":20, // User die ihren Status auf ONLINE haben
    "idle":5, // User die ihren Status auf IDLE haben
    "dnd":6, // User die ihren Status auf DND haben
    "offline":570, // User die ihren Status auf OFFLINE haben
    "difference":1 // Unterschied User gegenüber dem letztem Tag
}
```
{% endswagger-response %}
{% endswagger %}

{% swagger method="get" path="/messages" baseUrl="https://api.thedannicraft.de/data/discord/gamerforge" summary="" %}
{% swagger-description %}
Rufe Daten zu Message-Statistiken ab.
{% endswagger-description %}

{% swagger-response status="200: OK" description="ERFOLG" %}
```javascript
{
    "all":1929266, // Insgesammte Messages(seit Beginn des Trackings)
    "monthly":11491, // Messages diesen Monat
    "lastmonth":11739, // Messages letzten Monat
    "daily":53, // Heutige Messages
    "yesterday":358 // Gestrige Messages
}
```
{% endswagger-response %}
{% endswagger %}
