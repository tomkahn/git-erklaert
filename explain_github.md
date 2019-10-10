# Kollaboratives Arbeiten auf GitHub

## Git und GitHub

GitHub ist die größte Plattform, die es Developern, Engineers und Designern erlaubt ihre Arbeit zu teilen und im Team an einem Projekt zu arbeiten. Sie basiert auf git, dem version control system, welches jede Änderung in einer Datei nachverfolgen kann und es so möglich macht, nicht nur die komplette Historie einer Bearbeitung nachzuvollziehen, sondern darin auch zu erkennen, welcher Autor welchen Teil einer Datei verfasst hat.
Festzuhalten ist, dass git und GitHub nicht kongruent sind. Git ist das Werkzeug, welches Versionskontrolle ermöglicht. [GitHub](https://github.com/) ist eine Plattform auf der man Dateien (häufig Code) speichern und verwalten kann. Andere Anbieter sind [Gitlab](https://gitlab.com) oder [BitBucket](https://bitbucket.org/).

## Wie funktioniert die Versionskontrolle?

Wir alle kennen es: wir arbeiten an einem längeren Dokument und speichern immer wieder verschiedene Versionen ab.

Bachelorarbeit.docx
Bachelorarbeit_final.docx
Bachelorarbeit_final_final.docx
Bachelorarbeit_final_jetzt_aber_wirklich.docx

Keine besonders sichere Methode, um tatsächlich den letzten Stand eines Dokuments zu speichern. Noch komplizierter wird es, wenn nicht nur einzelne Bearbeiter, sondern ein ganzes Team an einem Dokument arbeitet. Wird dann nur einmal nicht die richtige Datei geteilt, geht wertvolle Arbeit verloren.

Git kann hier aushelfen. Jeder Arbeitsschritt, sei es ein fertiggestelltes Feature beim Coden oder ein Absatz beim Schreiben, sollte mit einem sogenannten _commit_ abgeschlossen werden. So wird der aktuelle Stand der Arbeit abgespeichert. Man kann sich eine Liste aller commits ansehen und seine Arbeit in den Stand vorheriger commits zurückversetzen. Dies ist insbesondere beim Programmieren von Vorteil, da nie sukkzessiv in einer einzelnen Datei gearbeitet wird, sondern jeweils in mehreren Dateien.
In einem commit wird nicht nur die aktuelle Version gespeichert, sondern auch die Zeit und der Bearbeiter.

GitHub kommt dann als neues Level zum Arbeitsprozess hinzu. Ein Ordner, mit Dateien auf dem eigenen Computer kann auf GitHub hochgeladen und dort verwaltet werden. Dieser Arbeitsschritt sollte ein- oder mehrmals am Tag durchgeführt werden. GitHub dient dabei auch als Backup, im Falle eines Problems mit der lokalen Datei. Im Fachjargon spricht man beim Hochladen von _pushen_, da der Befehl, der im Terminal ausgeführt wird, `git push` lautet. Ein Projekt auf GitHub wird in einem _repository_ gespeichert.

Aber auch ohne Programmierkenntnisse kann man sich an Projekten auf GitHub beteiligen. Das Userinterface von GitHub ermöglicht es. Siehe dazu unter (An diesem Projekt mitwirken)

## Versionskontrolle für Teamarbeit

Für die Teamarbeit an einem Projekt wird ein weiteres Konzept von git zur Hilfe genommen: branching. Für jedes Projekt gibt es eine Hauptversion, die _master branch_ heißt. Arbeiten verschiedene Autoren zusammen, kann keiner von ihnen mehr auf dem master branch arbeiten. Vielmehr muss jeder Autor einen eigenen _branch_ erstellen. Beim Programmieren lautet die Regel pro feature oder pro bug fix einen neuen branch zu benutzen.
Auf diesem branch wird dann gearbeitet, dort werden auch die commits erstellt und dieser branch wird gepusht.
Sobald ein Feature, bug fix oder Beitrag fertiggstellt wurde (mit regelmäßigen commits und pushes) kann ein _pull request_ erstellt werden. Damit gibt man anderen Projektmitarbeitern ein Zeichen, dass die Arbeit abgeschlossen ist. Sie wird dann zur Überprüfung freigestellt. In der Ansicht bei GitHub kann jede bearbeite Datei eingesehen werden, und es werden die Änderungen gegenüber dem master branch angezeigt.
Der Teamleader kann die Änderungen annehmen, indem er den pull request _mergt_, d.h. ihn mit dem master branch verschmilzt.
Der branch hat dann keine Bedeutung mehr und kann gelöscht werden. Für einen neuen Beitrag wird ein neuer branch kreiert.

Um eigene branches zu erstellen und an einem Coding-Projekt mitwirken zu können, muss zunächst eine lokale Kopie erstellt werden - dies nennt man _clonen_. Man kann dann lokal arbeiten und einen branch erstellen und ihn letztendlich pushen und einen pull request freischalten.
Eine andere Möglichkeit besteht darin, das komplette Projekt zu _forken_. Dabei wird das Projekt kopiert und als repository auf dem eigenen GitHub-Account angelegt. Von seinem Projekt kann man eigene branches erstellen, diese werden dann auch im Originalprojekt angezeigt und können direkt dort gemergt werden.

## An diesem Projekt mitwirken

Es bestehen zwei verschiedene Möglichkeiten, um am Open Source Legal Tech Lehrbuch mitzuarbeiten.
Einerseits können Beiträge eingereicht werden unter dieser Mailadresse: xxx@xxx.xxx

Für die direkte Mitarbeit auf GitHubv - was sich insbesondere bei kleinen Änderungen anbietet, sollten diese Schritte bfolgt werden:
1. Zunächst muss ein Account auf GitHub angelegt werden.
2. Forke das Projekt in deinen eigenen Account.
3. Erstelle einen neuen Branch.
4. Fertige Änderungen oder Ergänzungen an.
5. Commit und push.
6. Erstelle einen pull request im Originalprojekt.



