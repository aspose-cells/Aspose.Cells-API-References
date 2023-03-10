---
title: preferred_parsers Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 300
url: /de/python-net/aspose.cells/txtloadoptions/preferred_parsers/
is_root: false
---
##  preferred_parsers Eigentum

Ruft bevorzugte Wertparser zum Laden von Textdateien ab und legt diese fest.

###  Bemerkungen

parsers[0] ist der Parser, der für die erste Spalte in der Textvorlagendatei verwendet wird.
parsers[1] ist der Parser, der für die zweite Spalte verwendet wird, ...etc.
Die letzte (parsers[parsers.length-1]) wird für alle anderen Spalten verwendet, die bei parsers.length-1 beginnen.
Wenn ein Element null ist, wird die entsprechende Spalte vom Standardparser Aspose.Cells analysiert.
###  Definition:
```python
@property
def preferred_parsers(self):
    ...
@preferred_parsers.setter
def preferred_parsers(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [TxtLoadOptions](/cells/de/python-net/aspose.cells/txtloadoptions)
