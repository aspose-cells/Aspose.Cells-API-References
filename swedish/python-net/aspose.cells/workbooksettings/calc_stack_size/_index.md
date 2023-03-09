---
title: calc_stack_size fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 100
url: /sv/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size fastighet

Anger stackstorleken för att beräkna celler rekursivt.
Det stora värdet för denna storlek ger bättre prestanda när det finns många celler som måste beräknas rekursivt.
Å andra sidan kommer ett större värde att öka risken för StackOverflowException.
Om användaren får StackOverflowException vid beräkning av formler, bör detta värde minskas.

###  Anmärkningar

OBS: Denna medlem är nu föråldrad.
med den angivna CalcStackSize vid beräkning av formler.
 Den här egenskapen kommer att tas bort 12 månader senare sedan februari 2022.
Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.
###  Definition:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [WorkbookSettings](/cells/sv/python-net/aspose.cells/workbooksettings)
