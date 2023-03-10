---
title: set_license Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/license/set_license/
is_root: false
---
##  set_license(license_name) {#str}
Lizenziert die Komponente.



```python
def set_license(self, license_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| license_name | str |  |
###  Bemerkungen

Versucht, die Lizenz an den folgenden Orten zu finden:


1. Explizite Pfad.


2. Der Ordner, der die Komponentenbaugruppe Aspose enthält.


3. Der Ordner, der die aufrufende Assembly des Clients enthält.


4. Der Ordner, der den Eintrag (Startup) Assembly enthält.


5. Eine eingebettete Ressource in der aufrufenden Assembly des Clients.


**Notiz:** Versucht auf dem .NET Compact Framework, die Lizenz nur an diesen Orten zu finden:


1. Explizite Pfad.


2. Eine eingebettete Ressource in der aufrufenden Assembly des Clients.
###  Beispiel


In diesem Beispiel wird versucht, eine Lizenzdatei namens MyLicense.lic zu finden
 in dem Ordner, der enthält


die Komponente in dem Ordner, der die aufrufende Assembly enthält,
im Ordner der Eintragsassembly und dann in den eingebetteten Ressourcen der aufrufenden Assembly.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
Kann ein vollständiger oder kurzer Dateiname oder Name einer eingebetteten Ressource sein.
Verwenden Sie eine leere Zeichenfolge, um in den Bewertungsmodus zu wechseln.


##  set_license(stream) {#io.RawIOBase}
Lizenziert die Komponente.



```python
def set_license(self, stream):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Ein Stream, der die Lizenz enthält.|
###  Bemerkungen

Verwenden Sie diese Methode, um eine Lizenz aus einem Stream zu laden.
###  Beispiel


```python
from aspose.cells import License

license = License()
license.set_license(myStream)

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [License](/cells/de/python-net/aspose.cells/license)
