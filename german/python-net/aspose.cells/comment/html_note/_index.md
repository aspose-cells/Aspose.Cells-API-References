---
title: html_note Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 140
url: /de/python-net/aspose.cells/comment/html_note/
is_root: false
---
##  html_note Eigentum

Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formate in diesem Kommentar enthält.

###  Bemerkungen

Wenn es sich um einen Thread-Kommentar handelt, könnte die Notiz nicht geändert werden, da MS Excel ihn sonst nicht als Thread-Kommentar verarbeiten könnte.

###  Beispiele

```python

comment1.html_note = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Definition:
```python
@property
def html_note(self):
    ...
@html_note.setter
def html_note(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Comment](/cells/de/python-net/aspose.cells/comment)
