# Github-Flow Lesson: Der Weg zum perfekten Brownie 🍫👩‍🍳

Willkommen, liebe Back- und Code-Enthusiasten! 🎉 In dieser Lektion tauchen wir in die Welt des Github-Flows ein, um gemeinsam das ultimative Brownie-Rezept zu kreieren. Warum verbinden wir Backen mit Coden, fragt ihr euch? Weil beides kreative Prozesse sind, die von Teamarbeit, Präzision und natürlich von guten Rezepten bzw. guten Codes profitieren!

Stellt euch vor, ein weltbekannter Koch hat ein neues Brownie-Rezept veröffentlicht. Es klingt lecker, aber ihr habt das Gefühl, dass es noch verbessert werden könnte. In dieser Lektion werdet ihr lernen, wie ihr eure eigenen Änderungen an diesem Rezept vornehmen, sie mit anderen teilen und Feedback sammeln könnt, alles mit der Hilfe von Git und GitHub.

Bereit? Dann schnallt euch an, bindet die Schürzen um und öffnet eure Code-Editoren. Es wird lecker! 🍫👨‍💻

## Aufgabe 1: Repository klonen 🚀

Unser erster Stopp: Das Klonen dieses Repos auf euren Rechner. 
Schnappt euch die URL hinter dem grünen Button oben rechts auf der Repo-Seite und los geht's:

```powershell
git clone [Repository-URL]
```

### Ein kleiner Exkurs: Was machen `git clone`, `git pull` und `git push` eigentlich? 🤔

Stellt euch vor, ein weltbekannter Koch hat ein neues Brownie-Rezept veröffentlicht. Ihr seid total begeistert und wollt es unbedingt ausprobieren. Also holt ihr euch eine Kopie des Originalrezepts mit `git clone`. Jetzt könnt ihr zu Hause in Ruhe backen.

Bevor ihr jedoch die Schürze umbindet, bemerkt ihr, dass der Koch eine wichtige Änderung am Rezept vorgenommen hat. Ups, er hatte Esslöffel und Teelöffel vertauscht! Ihr aktualisiert eure Kopie des Rezepts mit `git pull`, um sicherzustellen, dass ihr die neueste und beste Version habt.

Ihr backt die Brownies und stellt fest, dass sie für euren Geschmack ein bisschen zu trocken sind. Also fügt ihr dem Rezept eine zusätzliche halbe Tasse Milch hinzu. Zufrieden mit eurer Verbesserung, teilt ihr sie, indem ihr sie "hochladet" mit `git push`. Jetzt können alle von eurer genialen Anpassung profitieren!

## Aufgabe 2: Feature-Branch erstellen 🌿

Ihr habt das Brownie-Rezept ausprobiert und festgestellt, dass der Teig ein bisschen zu trocken ist. Bevor wir diese bahnbrechende Erkenntnis nutzen um das Rezept anzupassen, brauchen wir einen eigenen Bereich für unsere Änderungen.

In der Git-Welt nennen wir das einen "Feature-Branch".

Führt den folgenden Befehl aus, um einen neuen Branch namens `feature/more-moisture` zu erstellen:

```powershell
git checkout -b feature/more-moisture
```

### Was ist ein Feature-Branch?

Stellt euch vor, ihr habt ein großes Puzzle, und jeder in eurem Team arbeitet an einem eigenen Teil davon. Ihr wollt nicht, dass eure Teile durcheinanderkommen, also arbeitet jeder an seinem eigenen kleinen Tisch (das ist euer "Feature-Branch"). Später fügt ihr alle Teile zusammen, um das große Gesamtbild zu sehen.
So könnt ihr sicherstellen, dass eure Änderungen isoliert sind und nicht den **Hauptzweig (`main`-Branch)** des Projekts stören, bis sie bereit für die große Bühne sind.

Perfekt, dann geht's weiter! 😊


## Aufgabe 3: Änderungen vornehmen und commiten 📝🎮

Ihr habt beschlossen dem Rezept `50ml` Milch hinzuzufügen, um die Brownies saftiger zu machen. 🥛🍫

Öffnet die `brownie-rezept.md`\-Datei und fügt `50ml Milch` zu den Zutaten hinzu. Speichert die Änderungen und führt dann die folgenden Befehle aus, um eure Änderungen zu commiten:

```powershell
git add brownie-rezept.md # markiert die Datei "brownie-rezept.md" für den nächsten Commit / Für die nächste Version
git commit -m "Added 50ml milk to make the brownies moister" # sichert alle mit `add` hinzugefügten Änderungen in einem neuen Commit / einer neuen Version
```

#### Was passiert hier? 🤔🎮

Stellt euch vor, ihr zockt ein Retro-Videospiel auf einem Emulator. Ihr habt gerade einen epischen Bosskampf gewonnen und ein neues Level erreicht. 🐉🏆 Anstatt nur einen einzigen Speicherstand zu überschreiben, nutzt ihr die "Save State"-Funktion des Emulators. Warum? Weil ihr damit mehrere "Save States" anlegen könnt! 🎉

Jeder "Save State" ist wie ein Commit in Git. Er speichert nicht nur euren aktuellen Fortschritt, sondern auch alle vorherigen "Save States". Das bedeutet, ihr könnt jederzeit zu einem früheren Zustand zurückkehren, sei es, um eine andere Strategie auszuprobieren oder einfach nur, um zu sehen, wie weit ihr gekommen seid. 🔄🕹

Das ist der Vorteil von mehreren "Save States" (oder Commits): Ihr habt eine vollständige Versionsgeschichte und könnt eure Entwicklung nachvollziehen. Es ist, als hättet ihr eine Zeitmaschine für euer Projekt! 🚀⏳

## Aufgabe 4: Push it to the Max! 🚀🥛

Ihr habt das Brownie-Rezept ausprobiert und festgestellt, dass es definitiv mehr Milch braucht. Ihr habt die Änderung in eurem lokalen "Kochbuch" (Repository) vorgenommen und mit einem "Save State" (Commit) festgehalten.

Jetzt ist es an der Zeit, diese lebensverändernde Erkenntnis mit der Welt zu teilen! 🌍🍫

Führt den folgenden Befehl aus:

```powershell
git push origin feature/more-moisture
```

### Was passiert hier? 🤔🥛

Ihr habt das Rezept ausprobiert und eine kleine, aber wichtige Änderung vorgenommen. Jetzt ist es an der Zeit, dieses aktualisierte Rezept der Welt zu präsentieren, damit niemand mehr unter trockenen Brownies leiden muss! 🌍🍫

Mit `git push` ladet ihr eure Änderungen in das Online-Repository hoch, genau wie ihr ein verbessertes Rezept auf einer Kochwebsite aktualisieren würdet. Jetzt können alle von eurer kulinarischen Weisheit profitieren! 🎉👩‍🍳

## Aufgabe 5: Pull Request -- Zeit für ein Review! 📝🔍

Jetzt, wo ihr eure Änderungen online gestellt habt, ist es an der Zeit, sie mit dem Originalrezept (dem `main`\-Branch) zu verschmelzen. Aber bevor das passiert, brauchen wir ein **Review**. Erstellt einen `Pull Request` (PR) und taggt mich `@EvilWeasel` für eine Überprüfung (`Review`) eurer Änderungen!

### Was passiert hier? 🤔🍪

Stellt euch vor, ihr habt euer verbessertes Brownie-Rezept online gestellt. Jetzt wollt ihr, dass es von der Koch-Community überprüft wird, bevor es das offizielle Rezept auf der Website ersetzt. 🌐👩‍🍳

Ein Pull Request ist wie eine Einladung zur Geschmacksprobe. Ihr bittet andere, eure Änderungen zu überprüfen und Feedback zu geben. Sobald alle zufrieden sind, wird das neue Rezept offiziell! 🎉🍫

#### So erstellt ihr einen Pull Request:

1.  **Geht zu eurem Repository auf GitHub.**
2.  **Klickt auf den Tab "Pull Requests".**
3.  **Klickt auf den grünen Button "New Pull Request".**
4.  **Wählt den `main`\-Branch als "base" und euren Feature-Branch `feature/more-moisture` als "compare".**
5.  **Überprüft die Änderungen und klickt dann auf "Create Pull Request".**
6.  **Gebt eurem Pull Request einen Titel und eine Beschreibung.**
7.  **Taggt mich (@EvilWeasel) im Kommentarfeld und bittet um eine Überprüfung eurer Änderungen.**
8.  **Klickt auf "Create Pull Request".**

Und voilà! Ihr habt euren ersten Pull Request erstellt und mich für ein Review getaggt! 🎉📝

Jetzt könnt ihr eure Änderungen mit anderen teilen und Feedback erhalten, bevor sie in das Originalrezept (den `main`\-Branch) übernommen werden. 🍪👨‍🍳

## Aufgabe 6: Code Review -- Die Geschmacksprobe 🍪👨‍🍳

Nachdem ihr euren Pull Request erstellt und mich (`@EvilWeasel`) für ein Review getaggt habt, ist es Zeit für ein Code Review. In dieser Phase überprüfe ich eure Änderungen, gebe Feedback und füge eine eigene, überprüfbare Änderung hinzu. Danach gebe ich meine Erlaubnis zum Mergen.

### Was passiert hier? 🤔🍴

Stellt euch vor, ihr habt eure Brownies zur Verkostung freigegeben. Jetzt kommen die anderen Köche und probieren sie. Sie geben euch Tipps, wie ihr das Rezept noch verbessern könnt. 🍫👩‍🍳

Ein Code Review ist wie diese Geschmacksprobe. Ihr bekommt Feedback zu eurem Code, könnt Fragen stellen und Diskussionen führen. Sobald alle zufrieden sind, wird das Rezept (der Code) für alle freigegeben! 🎉🍽

#### Wie führt man ein Code Review durch? 📝

1.  **Geht zu eurem offenen Pull Request auf GitHub.**
2.  **Scrollt nach unten zum Abschnitt "Reviewers" und fügt einen Reviewer hinzu.**
3.  **Wartet auf mein Feedback. Ich werde eine eigene Änderung vornehmen und den Merge freigeben.**
4.  **Beantwortet Fragen und führt eventuell notwendige Änderungen durch.**

#### Test: Überprüfung meiner Änderung 🧪

Der Test für diese Aufgabe prüft, ob meine spezifische Änderung im Commit vorhanden ist. Ich werde ein 🥛 Emoji in der `readme.md` hinzufügen. Wenn ihr diese Aufgabe selbst bearbeiten möchtet, stellt sicher, dass ihr diese Änderung auch vornehmt, damit der Test nicht fehlschlägt.

## Aufgabe 7: Merge -- Das Rezept wird offiziell! 🍪🎉

Jetzt, wo alle zufrieden sind und das Review abgeschlossen ist, wird es Zeit, eure Änderungen in den `main`\-Branch zu übernehmen. Das ist der Moment, in dem euer Rezept offiziell wird!

### Was passiert hier? 🤔👨‍🍳

Stellt euch vor, eure Brownies haben die Geschmacksprobe bestanden. Jetzt wird euer Rezept das offizielle Brownie-Rezept der Website. 🌐🍫

Das Mergen eines Pull Requests ist wie das Veröffentlichen eures Rezepts. Es wird Teil des offiziellen Kochbuchs und steht allen zur Verfügung. 📘👩‍🍳

#### Anleitung 📝

1.  **Geht zu eurem offenen Pull Request auf GitHub.**
2.  **Klickt auf den Button "Merge Pull Request", nachdem ich den Merge freigegeben habe.**
3.  **Bestätigt den Merge.**
4.  **Optional: Löscht den Feature-Branch, wenn ihr ihn nicht mehr benötigt.**

Und voilà, ihr habt es geschafft! Euer Rezept ist jetzt offiziell und jeder kann es nachkochen. 🎉🍽

## Abschluss der Lektion 🎉

### GitGraph Diagramm 📊

[![](https://mermaid.ink/img/pako:eNp1kk1OwzAQha9izTotSZy2qXdQfsSiG9ghb0zsJqbxOHIciVL1JCxYcT-OgOuC1Iri3cz7_Pw8mi1UVipgUGt_50TXMI6289piz3HLkYTDAQPz2IlKY82BkWySJsfSg5B66KOSctxxVCg5VtYY7YmWLGD3qL0WLVnEJgeOz05g1ZCVEn5w6sJYp0bG6n5fhcuNqtZ28P_qx-YLFyBFbg_o6Co67984oS6lJJPUtGSp2_VZ9evj853cGPuio_wbwQiNHI1ytTof58diGYm_KSCBcDm4yDDnOFMOvlFG7SfGQQoX4-wCJwZvHzdYAfNuUAkMnQw_u9aidsIAW4m2D91O4JO1JzWwLbwCy7LZeELn07IsyjnN85ImsAFGaTqmKU1TOs3LLCuyXQJv0SEbz_edSTGd0XxWFmmegJLaW7c87EVcj903OQ-4UA?type=png)](https://mermaid.live/edit#pako:eNp1kk1OwzAQha9izTotSZy2qXdQfsSiG9ghb0zsJqbxOHIciVL1JCxYcT-OgOuC1Iri3cz7_Pw8mi1UVipgUGt_50TXMI6289piz3HLkYTDAQPz2IlKY82BkWySJsfSg5B66KOSctxxVCg5VtYY7YmWLGD3qL0WLVnEJgeOz05g1ZCVEn5w6sJYp0bG6n5fhcuNqtZ28P_qx-YLFyBFbg_o6Co67984oS6lJJPUtGSp2_VZ9evj853cGPuio_wbwQiNHI1ytTof58diGYm_KSCBcDm4yDDnOFMOvlFG7SfGQQoX4-wCJwZvHzdYAfNuUAkMnQw_u9aidsIAW4m2D91O4JO1JzWwLbwCy7LZeELn07IsyjnN85ImsAFGaTqmKU1TOs3LLCuyXQJv0SEbz_edSTGd0XxWFmmegJLaW7c87EVcj903OQ-4UA)


### Git-Flow Recap 🔄

1.  **Repository klonen**: Wir haben das Repository auf unsere lokale Maschine geklont.
2.  **Feature-Branch erstellen**: Um sicherzustellen, dass wir isoliert arbeiten können, haben wir einen Feature-Branch namens `feature/more-moisture` erstellt.
3.  **Änderungen und Commits**: Wir haben das Brownie-Rezept angepasst, um den Teig weniger trocken zu machen, und diese Änderungen mit einem Commit festgehalten.
4.  **Push**: Die Änderungen wurden zum Remote-Repository gepusht.
5.  **Pull Request**: Ein Pull Request wurde erstellt, und ich wurde für ein Review getaggt.
6.  **Code Review und weitere Änderungen**: Während des Reviews habe ich ein 🥛 Emoji zur README hinzugefügt.
7.  **Merge**: Nach der Freigabe wurden die Änderungen in den `main`\-Branch gemerged.


