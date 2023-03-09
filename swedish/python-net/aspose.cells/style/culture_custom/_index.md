---
title: culture_custom fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells/style/culture_custom/
is_root: false
---
##  culture_custom fastighet

Hämtar och ställer in den kulturberoende mönstersträngen för talformat.
Om inget talformat har ställts in för detta objekt, returneras null.
Om talformat är inbyggt kommer mönstersträngen som motsvarar det inbyggda numret att returneras.

###  Anmärkningar

För inbyggt talformat är både mönsterinnehållet (t.ex. ett inbyggt datumformat "m/d/y" för vissa lokaler,
men för vissa andra lokaler blir det "d/m/y") och formatspecifikationen (som,
vissa lokaler använder ett annat tecken än 'y' för att representera årsdelen för datumformatering)
är kulturberoende;
För användarspecificerat anpassat format ändras endast formatspecifikationer enligt kulturen,
andra delar av formateringsmönstret kommer inte att ändras.
###  Definition:
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [Style](/cells/sv/python-net/aspose.cells/style)
