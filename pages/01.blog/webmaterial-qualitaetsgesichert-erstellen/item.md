---
title: 'Webmaterial qualitätsgesichert erstellen'
date: '26-02-2021 05:10'
hide_git_sync_repo_link: false
blog_url: /blog
show_sidebar: true
show_breadcrumbs: true
show_pagination: true
hide_from_post_list: false
feed:
    limit: 10
media_order: 'chelsea-scott-ml5TKVI2ys4-unsplash.jpg,test_structure.png'
hero_image: chelsea-scott-ml5TKVI2ys4-unsplash.jpg
taxonomy:
    category:
        - blog
    tag:
        - Material
        - Grav
        - Git
hero_classes: 'parallax text-light'
published: false
---

Ein ungelöstes Problem in der Erstellung von Materialien für den Schulunterricht, ist die langfristige _Maintenance_. Viele Lehrerinnen haben eine große Anzahl von Dateien, die früher oder später _out of date_ sind oder aber Fehler enthalten, die über Jahre hinweg möglicherweise nicht adressiert werden. Um diese Art und Weise der lehrerzentrierten Materialerstellung zu verändern, möchte ich hier ein Beispiel mit GravCMS und Git vorstellen. 

===

## Webmaterial qualitätsgesichert erstellen

Es gibt zahlreiche Möglichkeiten, um die hier vorgestellte Variante der Materialerstellung zu realisieren. Ich habe mich für GravCMS entschieden, da es aus meiner Perspektive die beste _authoring experience_ und technische Grundlage hat. 

Materialien sind oft direkt im schulischen Cloud-Storage als PDF oder in Moodle Kursen als PDF, selten aber als echtes Webmaterial zu finden ist. Eine Vermutung, die sich mir in den letzten Jahren immer mehr aufdrängt ist, dass ein geordneter Prozess für die Erstellung von Materialien geschaffen werden muss, der eine langjährige Entwicklung in Augenschein nimmt. Programmierer im Bereich der OpenSource Entwicklung machen dies oft, indem Sie Repositories eröffnen, in denen alle Prozesse der Veränderung festgehalten, erlaubt, abgelehnt und oder Änderungsvorschläge diskutiert werden. Ein Repository erlaubt es auch geklont und auf Basis seiner Lizenz verändert zu werden, gleichzeitig aber, wenn gewünscht, von Veränderungen des geklonten Repositories zu erben. Übertragen auf Materialien in der Schule bedeutet dies, dass man bei einer langfristig angelegten Planung von Materialpools in Schulen ein System schaffen kann, das einen so genannten _main branch_ (Hauptzweig) zusammen über eine Fachkonferenz für das Fach und bestimmte Jahrgänge pflegt, d.h. also ein Basis-Material für alle Kolleginnen zur Verfügung stellt, welches daraufhin aber kopiert und verändert werden kann, d.h. also weitere Zweige vom _main branch_ bilden kann.

![](test_structure.png)

Diese Arbeitsweise ist nicht unbekannt, allerdings in der Schule auf technischer Ebene selten oder nie angekommen. Hier arbeiten Individuen oft aneinander vorbei, da individuelle Herangehensweisen an Themen im Vordergrund stehen. Dies kann im Rahmen der Bearbeitung mit Grav und Git auch weiter so geschehen, da ja nur vom _main branch_ geerbt wird. Eine Einigung ist also nur auf Ebene der Fachkonferenz nötig. In der Praxis aufgefallene Fehler oder Verbesserungsvorschläge können als Pull-Request an den _main branch_ gestellt werden – die Fachkonferenz müsste dann entscheiden, ob dieser Änderungsvorschlag übernommen werden sollte oder nicht. Angenommen, eine Änderung wird im Nachhinein als problematisch empfunden, kann selbige per Git zurückverfolgt und der alte Zustand wiederhergestellt werden, da Git automatisiert eine Versionierung der synchronisierten Dateien vornimmt. 

Die Dateien, die synchronisiert werden sind in Markdown verfasst  _(*.md)_ diese vereinfachte HTML Darstellung ermöglicht es durch einfache Befehle Seiten zu erstellen. Markdown übersteigt jedoch die Fähigkeiten vieler Lehrer:innen. Grav CMS bietet hier mit einem Pro-Plugin (50$ pro Projekt) namens NextGen Editor eine kostengünstige Alternative, die das Verfassen von Markdown Dateien in einen WYSIWYG (What you see is what you get) Editor ermöglicht.

![NextGen](https://getgrav.org/user/pages/premium/nextgen-editor/markup.gif?g-fad0e05c)

Der NextGen Editor ermöglicht es Lehrer:innen (mit wenigen Ausnahmen) wie aus Textverarbeitungsprogrammen gewohnt ihr Material zu erstellen. Es wird jedoch als Markdown gespeichert und automatisiert in das Git-Repository synchronisiert, d.h. alle Änderungen werden automatisch in einen Zweig des Hauptzweiges übernommen, oder bei Bearbeitung des Hauptzweiges, direkt in den Hauptzweig übernommen werden. Diese ein wenig technische Beschreibung ist für die User eventuell unnötig, aber es ist wichtig, um zu verstehen, wie langfristig gute Materialien entstehen könnten, die trotz divergierender Varianten ganz konkret auf einem gemeinsamen Standard aufbauen, der über eine Fachkonferenz demokratisch und mit Blick auf die Kernlehrpläne und schulinterne Curricula entschieden wurde. 


