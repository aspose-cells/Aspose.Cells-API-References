---
title: enable_calculation_chain proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain proprietà

Se abilitare la catena di calcolo per le formule. L'impostazione predefinita è false.

###  Osservazioni

Quando ci sono molte formule nella cartella di lavoro e l'utente deve calcolarle ripetutamente
modificandone solo una piccola parte, può essere utile per le prestazioni abilitare la catena di calcolo.
D'altra parte, se la catena è abilitata, il mantenimento del modello di catena richiede memoria aggiuntiva,
e richiede anche un po' più di tempo della CPU per alcune altre operazioni come la modifica del valore o delle formule della cella.
Dopo aver modificato questa proprietà da false a true, la catena di calcolo verrà analizzata e costruita
al momento del primo calcolo per la cartella di lavoro, quindi il tempo richiesto per il primo calcolo
può essere più del normale calcolo senza catena.
###  Definizione:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [FormulaSettings](/cells/it/python-net/aspose.cells/formulasettings)
