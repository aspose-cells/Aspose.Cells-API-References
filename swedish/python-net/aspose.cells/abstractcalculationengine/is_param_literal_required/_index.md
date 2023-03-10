---
title: is_param_literal_required fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
##  is_param_literal_required fastighet

Indikerar om denna motor behöver den bokstavliga texten av parametern när den gör beräkningar. Standardvärdet är falskt.

###  Anmärkningar

Om den här anpassade beräkningsmotorn kräver parameterns bokstavliga text, kommer fler stackar att krävas för att cachelagra den bokstavliga texten för parametrar och metoden Calculate() kan anropas rekursivt för att beräkna parameterns värde.
Vanligtvis behövs inte den bokstavliga texten för att beräkna formler och denna metod bör returnera falskt för de flesta implementeringar för att få bättre prestanda.
###  Definition:
```python
@property
def is_param_literal_required(self):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [AbstractCalculationEngine](/cells/sv/python-net/aspose.cells/abstractcalculationengine)
