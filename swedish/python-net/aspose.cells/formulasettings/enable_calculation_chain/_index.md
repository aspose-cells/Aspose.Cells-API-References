---
title: enable_calculation_chain fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain fastighet

Om aktivera beräkningskedja för formler. Standard är falskt.

###  Anmärkningar

När det finns massor av formler i arbetsboken och användaren behöver beräkna dem upprepade gånger
Om du bara ändrar en liten del av dem kan det vara till hjälp för prestanda att aktivera beräkningskedjan.
Å andra sidan, om kedjan är aktiverad kräver underhåll av kedjans modell extra minne,
och det kräver också lite mer cpu-tid för vissa andra operationer som att ändra cellens värde eller formler.
Efter att ha ändrat den här egenskapen från falsk till sann, kommer beräkningskedjan att analyseras och byggas
vid tidpunkten för första beräkningen för arbetsboken, så den tid som krävs för den första beräkningen
kan vara mer än normal beräkning utan kedja.
###  Definition:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [FormulaSettings](/cells/sv/python-net/aspose.cells/formulasettings)
