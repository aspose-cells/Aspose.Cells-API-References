---
title: calc_stack_size fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size fastighet

Anger stackstorleken för att beräkna celler rekursivt.

###  Anmärkningar

När det finns stora mängder celler måste beräknas rekursivt i beroendeträdet,
StackOverflowException kan orsakas i beräkningsprocessen.
Om så är fallet bör användaren ange ett mindre värde för den här egenskapen.
För sådana situationer bör användaren bestämma rätt värde för den här egenskapen enligt de faktiska formlerna och data.
För små värden kan orsaka prestandaförsämring för formelberäkningen.
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
* klass [CalculationOptions](/cells/sv/python-net/aspose.cells/calculationoptions)
