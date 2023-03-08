---
title: remove_at Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Entfernt den angegebenen externen Link aus der Arbeitsmappe.



```python
def remove_at(self, index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| index | int | der Index des externen Links, der entfernt werden soll.|
###  Bemerkungen

Beim Entfernen des externen Links werden auch alle darauf verweisenden Formeln entfernt, weil
die Verweise werden ungültig.

##  remove_at(index, update_references_as_local) {#int-bool}
Entfernt den angegebenen externen Link aus der Arbeitsmappe.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| index | int | der Index des externen Links, der entfernt werden soll.|
| update_references_as_local | bool | Ob alle Referenzen des angegebenen externen Links auf die Referenz der aktuellen Arbeitsmappe selbst aktualisiert werden.|
###  Bemerkungen

Wenn Verweise aktualisiert werden müssen, werden Verweise auf externe Links in Formeln in die aktuelle Arbeitsmappe geändert.
Der zu entfernende externe Link ist beispielsweise „externalsource.xlam“ und definiert eine benutzerdefinierte Funktion „customfunction()“.
Die ursprüngliche Formel einer Zelle lautet "='externalsource.xlam'!customfunction()",
Nach dem Entfernen wird die Formel zu "=customfunction()".
Wenn Verweise nicht aktualisiert werden müssen, alle Formeln mit Verweis auf diesen externen Link
werden ebenfalls entfernt, da diese Verweise ungültig werden.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [ExternalLinkCollection](/cells/de/python-net/aspose.cells/externallinkcollection)
