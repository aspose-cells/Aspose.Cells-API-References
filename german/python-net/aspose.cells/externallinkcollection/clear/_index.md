---
title: clear Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Entfernt alle externen Links.



```python
def clear(self):
    ...
```


###  Bemerkungen

Beim Entfernen externer Links werden auch alle darauf verweisenden Formeln entfernt, weil
die Verweise werden ungültig.

##  clear(update_references_as_local) {#bool}
Entfernt alle externen Links.



```python
def clear(self, update_references_as_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| update_references_as_local | bool | Ob alle Referenzen externer Links als Referenzen der aktuellen Arbeitsmappe selbst aktualisiert werden.|
###  Bemerkungen

Wenn Verweise aktualisiert werden müssen, werden Verweise auf externe Links in Formeln in die aktuelle Arbeitsmappe geändert.
Beispielsweise lautet die ursprüngliche Formel einer Zelle "='externalsource.xlam'!customfunction()",
Nach dem Entfernen externer Links wird die Formel zu „=customfunction()“.
Wenn Verweise nicht aktualisiert werden müssen, alle Formeln mit Verweisen auf externe Links
werden ebenfalls entfernt, da diese Verweise ungültig werden.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [ExternalLinkCollection](/cells/de/python-net/aspose.cells/externallinkcollection)
