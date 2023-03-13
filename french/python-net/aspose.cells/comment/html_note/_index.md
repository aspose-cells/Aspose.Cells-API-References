---
title: html_note propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 140
url: /fr/python-net/aspose.cells/comment/html_note/
is_root: false
---
##  html_note propriété

Obtient et définit la chaîne html qui contient des données et certains formats dans ce commentaire.

###  Remarques

S'il s'agit d'un commentaire fileté, la note ne pourrait pas être modifiée, sinon MS Excel ne pourrait pas la traiter comme un commentaire fileté.

###  Exemple

```python

comment1.html_note = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
###  Définition:
```python
@property
def html_note(self):
    ...
@html_note.setter
def html_note(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Comment](/cells/fr/python-net/aspose.cells/comment)
