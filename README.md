# Einführung in die Authentifizierung

Dieses Mal werden wir uns mit dem Thema Authentifizierung beschäftigen. Und das ist etwas, das oft als unglaublich kompliziert angesehen wird, aber das muss es nicht sein. Wir werden Schritt für Schritt von Anfang bis Ende vorgehen, so dass Sie einen Überblick über den gesamten Prozess der Einrichtung der Authentifizierung von Grund auf erhalten.

## Warum brauchen wir also eine Authentifizierung?

Nun, wenn wir unsere Website oder Webanwendung für die Benutzer erstellen, werden diese Benutzer anfangen, Daten auf der Website zu generieren. Vielleicht gefallen ihnen bestimmte Beiträge, vielleicht interagieren sie mit anderen Nutzern, vielleicht werden Nachrichten oder Rezepte erstellt. Es werden immer einige Benutzerdaten erstellt. Um diese Daten mit den einzelnen Nutzern in Verbindung zu bringen, müssen wir für jeden Nutzer ein Konto erstellen, damit er sich mit einem Benutzernamen und einem Passwort auf unserer Website anmelden kann, und wir erstellen für ihn eine Art Ausweis, um ihn in unserer Datenbank eindeutig zu identifizieren und alle von ihm erzeugten Daten in diesem Konto zu speichern. Wenn sie also das nächste Mal auf die Website zurückkehren, können sie sich mit ihrem Benutzernamen und Passwort auf unserer Website anmelden und auf all diese möglicherweise privaten Informationen zugreifen. Auf diese Weise kann nicht jeder sehen, welche privaten Nachrichten Sie auf Facebook verschicken oder welche Direktnachrichten Sie auf Twitter verschicken.

Das ist also ziemlich einfach.

Ein weiterer Grund, warum Sie Ihrer Website eine Authentifizierung hinzufügen sollten, ist die Einschränkung des Zugriffs auf bestimmte Bereiche der Website in Abhängigkeit vom Status des Benutzers. Wenn Sie z. B. Spotify oder Netflix wären und für den Zugriff auf bestimmte Bereiche der Website ein Abonnement verlangen, dann müssen Sie, sobald der Benutzer bezahlt hat, sein Konto in Ihrer Datenbank aktualisieren, um zu vermerken, dass er bezahlt hat, und ihm den Zugriff auf die Fernsehsendungen oder Musiktitel gewähren, auf die er Anspruch hat.

Das sind also einige der Gründe, warum Sie Ihre Website mit einer Authentifizierung ausstatten sollten. Die Authentifizierung kann jedoch auf verschiedene Weise erfolgen. Eine Website zu erstellen, auf der sich Benutzer anmelden und einloggen können, scheint einfach genug zu sein, aber der schwierige Teil der Authentifizierung liegt darin, wie sicher Sie Ihre Website machen wollen. Und wir werden dieses Problem der Authentifizierung angehen, indem wir die verschiedenen Sicherheitsstufen durchgehen. Wir werden also von der grundlegenden Erstellung eines Kontos, dem Hinzufügen des Benutzers zu unserer Datenbank, dem Speichern des Benutzernamens und des Passworts, damit er sich anmelden kann, bis hin zu Dingen wie OAuth und Social Logins gehen, einschließlich der Erstellung von Dingen wie Sitzungen und Cookies und Hashing und Verschlüsselung von Passwörtern. Es wird mehr sein, als Sie jemals über dieses Thema wissen wollen, aber es ist wirklich sehr wichtig, dass Sie es am Anfang lernen, denn später, wenn Sie es verstanden haben und die Authentifizierung von Grund auf aufgebaut haben, werde ich Ihnen einige Möglichkeiten zeigen, wie Sie Ihr Leben mit Bibliotheken von Drittanbietern wie Passport vereinfachen und erleichtern können. Wir werden also lernen, wie man von einer Website, die im Wesentlichen mit einem chito
![chito](./images/chito.png)
 zu etwas, das viel seriöser ist und mehr den Industriestandards für gute Sicherheit auf einer Website entspricht.


Es gibt eine App namens Whisper, auf die Sie vielleicht schon gestoßen sind, und es ist ein wirklich einfaches Konzept, das es den Leuten ermöglicht, ihre Geheimnisse anonym zu veröffentlichen. Was auch immer sie posten, ist also nicht mit einer E-Mail oder einem Benutzernamen verbunden, und das bedeutet, dass die Leute sich freier ausdrücken können, denke ich. Die Struktur unserer Website ist also wirklich sehr einfach. Es gibt eine Startseite mit zwei Schaltflächen, über die man sich entweder registrieren oder anmelden kann, und sobald der Benutzer registriert oder angemeldet ist und sich authentifiziert hat, kann er auf die Seite mit den Geheimnissen zugreifen.

![whisper](./images/whisper.png)


Ich habe den Rest der Website ziemlich einfach gehalten, weil wir uns auf ein ziemlich komplexes Thema konzentrieren werden, damit wir uns auf das Erlernen der Authentifizierung konzentrieren können und nicht durch Dinge wie Bootstrap und Styling abgelenkt werden.
