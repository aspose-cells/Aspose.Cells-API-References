---
title: html_note proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 140
url: /it/python-net/aspose.cells/comment/html_note/
is_root: false
---
##  html_note proprietà

Ottiene e imposta la stringa html che contiene dati e alcuni formati in questo commento.

###  Osservazioni

Se si tratta di un commento con thread, la nota non può essere modificata, altrimenti MS Excel non potrebbe elaborarla come commento con thread.

###  Esempi

```python

comment1.html_note = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Definizione:
```python
@property
def html_note(self):
    ...
@html_note.setter
def html_note(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Comment](/cells/it/python-net/aspose.cells/comment)
