---
title: check_font_compatibility fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility fastighet

Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.

###  Anmärkningar

Standardvärdet är sant.
Inaktivera den här egenskapen kan ge bättre prestanda.
Men när standard eller specificerat teckensnitt för text/tecken inte kan användas för att återge det,
oläsbara tecken (som block) kan förekomma i den genererade pdf-filen.
För en sådan situation bör användaren behålla denna egenskap som sann så att
alternativt teckensnitt kan sökas och användas för att återge texten istället;
###  Definition:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [PptxSaveOptions](/cells/sv/python-net/aspose.cells/pptxsaveoptions)
