---
title: check_font_compatibility Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility Eigentum

Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.

###  Bemerkungen

Der Standardwert ist wahr.
Deaktivieren Sie diese Eigenschaft, um eine bessere Leistung zu erzielen.
Aber wenn die Standard- oder angegebene Schriftart von Text/Zeichen nicht zum Rendern verwendet werden kann,
Im generierten PDF können unlesbare Zeichen (z. B. Block) auftreten.
Für eine solche Situation sollte der Benutzer diese Eigenschaft auf true belassen
alternative Schriftarten können gesucht und stattdessen zum Rendern des Textes verwendet werden;
###  Definition:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PdfSaveOptions](/cells/de/python-net/aspose.cells/pdfsaveoptions)
