---
title: is_gather_string Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Überprüft, ob der aktuelle Zeichenfolgenwert der Zelle in einem globalen Pool gesammelt werden muss.


###  Kehrt zurück

wahr, wenn der Zeichenfolgenwert für die resultierende Datei in einem globalen Pool gesammelt werden muss.


```python
def is_gather_string(self):
    ...
```


###  Bemerkungen

Das Sammeln von Zeichenfolgenwerten wird nur dann Vorteile bringen, wenn viele duplizierte Zeichenfolgenwerte für die von dieser Implementierung bereitgestellten Zellen vorhanden sind.
In dieser Situation spart das Sammeln von Zeichenfolgen viel Speicherplatz und erzeugt eine kleinere resultierende Datei.
Wenn es viele Zeichenfolgenwerte für die von LightCellsDataProvider bereitgestellten Zellen gibt, aber nur wenige davon gleich sind,
Das Sammeln von Zeichenfolgen kostet mehr Speicher und Zeit und hat keinen Vorteil für die resultierende Datei.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [LightCellsDataProvider](/cells/de/python-net/aspose.cells/lightcellsdataprovider)
