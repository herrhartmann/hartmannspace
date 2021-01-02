---
title: 'Technologische Grundlagen und philosophische Grundfragen für offenes Webmaterial'
feed:
    limit: 10
media_order: brina-blum-Bb_X4JgSqIM-unsplash.jpg
publish_date: '13-12-2020 09:38'
metadata:
    Unterricht: Didaktik
    Digitalisierung: ''
taxonomy:
    category:
        - blog
    tag:
        - Unterricht
        - Didaktik
dateformat: 'd-m-Y H:i'
hero_classes: 'parallax text-light overlay-dark hero-large'
hero_image: brina-blum-Bb_X4JgSqIM-unsplash.jpg
---

In diesem Blogartikel möchte ich erklären, wie offenes Material auf Ebene der Administration angeboten und für User aufbereitet werden kann. Gleichzeitig biete ich Beispiele dafür auf meiner Website an, um es auch den Anwendern möglich zu machen, diese Gedanken nachzuvollziehen. Offen bedeutet für mich: (1) es handelt sich um OER, welches direkt in einem CMS erstellt ist (in meinem Falle GravCMS) (2) das Material kann per 2-way-sync zwischen der Website und Github/Gitea synchronisiert werden, wobei eine Versionskontrolle stattfindet. (3) Es gibt ein Materialverzeichnis - in diesem Falle mit Flex-Objects, welches das Durchsuchen unheimlich schnell und effizient macht.

===

Eine Frage, die ich mir bei der Bedienung von großen LMS immer stelle ist, wofür die Komplexität vieler Systeme in Bezug auf die Erstellung von Materialien überhaupt notwendig ist. Eine basale Anforderung an Webmaterial ist, dass medienkonvergente Inhalte gut aufbereitet, barrierefrei, responsiv und effizient abrufbar sind. Viele LMS scheitern schon an einem zu komplexen User-Interface mit verschachtelten Menüs und Optionen, ganz abgesehen von individuellen User-Logins und der Implementation von Dritttools für die Erstellung interaktiver Inhalte. Im Alltag vieler Lehrer:innen ist mangels Zeit und oft auch mangels Kenntnissen im Bereich der Bearbeitung, der Berücksichtigung von Datenschutz und Urheberrecht keine Zeit für ein effizientes Erstellen von Online-Material. Dieser Umstand führt dazu, dass komplexe LMS mit PDFs gefüllt werden. Für die Erstellung von gutem online Material setze ich auf moderne Flatfile CMS. 

> Keep it simple!

Das Motto hierbei lautet für mich: "Keep it simple". Das Material sollte binnen Minuten erstellbar, distribuierbar und ohne Umstände für alle erreichbar sein. 

Wie das genau funktioniert, und warum es notwendig ist, möchte ich hier kurz erklären. Viele LMS sind in der Regel geschlossen und bieten verschiedenste Testformate an, die oft von Plugins oder Drittanbietern abhängig sind. Oft frage ich mich, ob das wirklich notwendig ist, um gute Materialien für den Unterricht zu erstellen. Im Rahmen der Digitalisierungsdebatte wird oft von personalisierten Lernszenarien gesprochen - was ich aber oft vorfinde sind standardisierte Tests mit wenig Involvement und viel PDF - Lehrer:innen versuchen Ihr bestes, machen aber oft auch Ihre ersten Gehversuche im Netz. Ich möchte hier vorstellen, wie man einfache Lernsettings in einem CMS mit einfachen Kniffen personalisieren kann, ohne dabei komplexe Strukturen erlernen zu müssen. Die empirischen Befunde zu Online-Testverfahren sind oft uneindeutig, die 
