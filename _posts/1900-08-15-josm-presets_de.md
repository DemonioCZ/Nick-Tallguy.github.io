---
layout: doc
title: JOSM Vorlagen
permalink: /de/josm/josm-presets/
lang: de
category: josm
---

JOSM Vorlagen
============

> Diese Anleitung kann heruntergeladen werden als [josm-presets_en.odt](/files/josm-presets_en.odt) or [josm-presets_en.pdf](/files/josm-presets_en.pdf)  
> Reviewed 2016-09-17  

Wenn man JOSM schon etwas länger verwendet, versteht man etwas von Tags und Vorlagen. Jedes Objekt wird durch zwei Dinge definiert - als erstes durch seine Geometrie (ob es ein Punkt, eine Linie oder ein Umriss ist und sein Standort) und zweitens durch seine Attribute in Form von Tags.  

Wenn man ein Objekt mittels Vorlagenmenü zeichnet, werden die korrekten Tags automatisch dem Objekt zugeordnet.  

Was passiert, wenn man Tags trotz der Verwendung von Vorlagen hinzufügen möchte, die nicht im Menü enthalten sind oder man eigene Tags anpassen möchte?  

In diesem Fall kann man eigene Menüeintrage den Vorlagen hinzufügen. In diesem Abschnitt befassen wir uns damit. Im [folgenden Kapitel](/de/editing/creating-presets) werden wir uns mit dem Erstellen von eigenen Vorlagen befassen.  


Vorlagen hinzufügen
-----------

Die Menüs und Untermenüs des Vorlagenmenüs sind in Dateien gespeichert, die beschreiben, wie Menüs und Formulare erstellt werden, wenn man auf eine Vorlage klickt und welche Tags einem Objekt hinzugefügt werden, je nachdem wie das Formular ausgefüllt wird.  

Vorlagen können entweder von einer Onlinebibliothek aus oder lokal gespeichert und hinzugefügt werden in JOSM.  

* Um einen neuen Eintrag dem Vorlagenmenu hinzuzufügen, öffnet man JOSM und geht zu Bearbeiten->Einstellungen.  
* Man klickt auf das dritte Tab, das wie ein Gitter über einem Planeten aussieht.  

![tagging presets tab][]

* Oben klickt man auf "Tagging Vorlagen".  

![tagging presets menu][]

* Man fügt eine Vorlage aus dem Internet hinzu durch Auswahl in der Liste 	zur Linken und durch klicken auf den blauen Pfeil. In diesem Beispiel 	fügen wir die Vorlage "Buildings Indonesia by Kate Chapman" hinzu.  

![example presets][]

* Man sieht einen neuen Eintrag erscheinen in der Liste auf der rechten Seite.  
* Man klickt OK.  
* Man startet JOSM neu.  
* Man erstellt einen neuen Layer und fügt einen Punkt oder Umriss hinzu.  
* Man geht ins Vorlagenmenü. Man klickt auf den Eintrag "Building", welches am Ende des Menüs hinzugefügt wurde.  

![indonesia building form][]

* Falls man kein indonesisch spricht, wird es schwer zu lesen sein, aber man hat trotzdem erfolgreich ein eigenes Vorlagenmenü hinzugefügt.  

* Falls man eine angepasste Vorlagendatei bekommen hat, kann man es auf ähnlichem Weg dem Menü hinzufügen. Man kehrt zurück zum Einstellungen Menü und anstatt dass man etwas in der Liste auswählt, klickt man auf den (+) Button oben rechts.  

![plus button][]

* Man sucht die Datei und gibt ihr gegebenenfalls einen Namen.  
* Man klickt OK.  


[tagging presets tab]: /images/josm/tagging-presets-tab.png
[tagging presets menu]: /images/josm/tagging-presets-menu.png
[example presets]: /images/josm/example-presets.png
[indonesia building form]: /images/josm/indonesia-building-form.png
[plus button]: /images/josm/plus-button.png

