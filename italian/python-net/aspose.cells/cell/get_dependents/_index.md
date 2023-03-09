---
title: metodo get_dependents
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 90
url: /it/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella.



```python
def get_dependents(self, is_all):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| is_all | bool | Indica se controllare le formule in altri fogli di lavoro|
###  Osservazioni

* Se un riferimento contenente questa cella appare nella formula di una cella, quella cella verrà considerata come

il dipendente di questa cella, indipendentemente dal riferimento o questa cella viene utilizzata o meno durante il calcolo.
Ad esempio, sebbene la cella A2 nella formula "=IF(TRUE,A1,A2)" non venga utilizzata durante il calcolo,
questa formula è ancora da considerare come dipendente da A2.
Per ottenere quelle formule i cui risultati calcolati dipendono da questa cella, utilizzare [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation). Quando si tracciano i dipendenti per una cella, tutte le formule nella cartella di lavoro o nel foglio di lavoro verranno analizzate e controllate.
Quindi è un processo che richiede tempo. Se l'utente ha bisogno di tracciare i dipendenti per molte celle, l'utilizzo di questo metodo lo farà
causare scarse prestazioni. Per considerazioni sulle prestazioni, l'utente deve utilizzare invece [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation).
Oppure, l'utente può raccogliere prima la mappa precedente di tutte le celle entro [Cell.get_precedents()](/cells/it/python-net/aspose.cells/cell/get_precedents),
e quindi costruire la mappa dei dipendenti secondo la mappa dei precedenti.

* Se un riferimento contenente questa cella appare nella formula di una cella, quella cella verrà considerata come
il dipendente di questa cella, indipendentemente dal riferimento o questa cella viene utilizzata o meno durante il calcolo.
Ad esempio, sebbene la cella A2 nella formula "=IF(TRUE,A1,A2)" non venga utilizzata durante il calcolo,
questa formula è ancora da considerare come dipendente da A2.
Per ottenere quelle formule i cui risultati calcolati dipendono da questa cella, utilizzare [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation). Quando si tracciano i dipendenti per una cella, tutte le formule nella cartella di lavoro o nel foglio di lavoro verranno analizzate e controllate.
Quindi è un processo che richiede tempo. Se l'utente ha bisogno di tracciare i dipendenti per molte celle, l'utilizzo di questo metodo lo farà
causare scarse prestazioni. Per considerazioni sulle prestazioni, l'utente deve utilizzare invece [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation).
Oppure, l'utente può raccogliere prima la mappa precedente di tutte le celle entro [Cell.get_precedents()](/cells/it/python-net/aspose.cells/cell/get_precedents),
e quindi costruire la mappa dei dipendenti secondo la mappa dei precedenti.

* Se un riferimento contenente questa cella appare nella formula di una cella, quella cella verrà considerata come
il dipendente di questa cella, indipendentemente dal riferimento o questa cella viene utilizzata o meno durante il calcolo.
Ad esempio, sebbene la cella A2 nella formula "=IF(TRUE,A1,A2)" non venga utilizzata durante il calcolo,
questa formula è ancora da considerare come dipendente da A2.
Per ottenere quelle formule i cui risultati calcolati dipendono da questa cella, utilizzare [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation). Quando si tracciano i dipendenti per una cella, tutte le formule nella cartella di lavoro o nel foglio di lavoro verranno analizzate e controllate.
Quindi è un processo che richiede tempo. Se l'utente ha bisogno di tracciare i dipendenti per molte celle, l'utilizzo di questo metodo lo farà
causare scarse prestazioni. Per considerazioni sulle prestazioni, l'utente deve utilizzare invece [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation).
Oppure, l'utente può raccogliere prima la mappa precedente di tutte le celle entro [Cell.get_precedents()](/cells/it/python-net/aspose.cells/cell/get_precedents),
e quindi costruire la mappa dei dipendenti secondo la mappa dei precedenti.
###  Esempio

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
