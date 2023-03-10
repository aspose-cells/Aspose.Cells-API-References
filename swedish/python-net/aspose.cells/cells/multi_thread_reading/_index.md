---
title: multi_thread_reading fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1200
url: /sv/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading fastighet

Hämtar eller ställer in om celldatamodellen ska stödja multitrådsläsning.
Standardvärdet för den här egenskapen är falskt.

###  Anmärkningar

Om det finns flera trådar att läsa Row/Cell-objekt i den här samlingen samtidigt,
den här egenskapen bör ställas in som sann, annars kan oväntade resultat uppstå.
Stöd för flertrådsläsning kan försämra prestandan för åtkomst av Row/Cell-objekt från den här samlingen.
Observera att vissa funktioner inte stöder multitrådsläsning,
såsom formateringsvärden (med [Cell.string_value](/cells/sv/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/sv/python-net/aspose.cells/cell#display_string_value), .etc.).
Så även om den här egenskapen är inställd som sann, kan dessa API:er fortfarande ge oväntade resultat för flertrådsläsning.
###  Definition:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
