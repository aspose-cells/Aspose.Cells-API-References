---
title: calc_stack_size proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size proprietà

Specifica la dimensione dello stack per il calcolo delle celle in modo ricorsivo.
Il valore elevato per questa dimensione darà prestazioni migliori quando ci sono molte celle che devono essere calcolate in modo ricorsivo.
D'altra parte, un valore maggiore aumenterà il rischio di StackOverflowException.
Se l'utente ottiene StackOverflowException durante il calcolo delle formule, questo valore deve essere ridotto.

###  Osservazioni

NOTA: questo membro è ora obsoleto.
con il CalcStackSize specificato durante il calcolo delle formule.
 Questa proprietà verrà rimossa 12 mesi dopo da febbraio 2022.
Aspose si scusa per gli eventuali disagi causati.
###  Definizione:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [WorkbookSettings](/cells/it/python-net/aspose.cells/workbooksettings)
