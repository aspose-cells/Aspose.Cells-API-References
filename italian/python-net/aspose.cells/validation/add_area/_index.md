---
title: metodo add_area
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Applica la convalida all'area.



```python
def add_area(self, cell_area):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| cell_area | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | L'area.|
###  Osservazioni

Equivale a utilizzare [Validation.add_area(cell_area)](/cells/it/python-net/aspose.cells/validation/add_area)
con controllo intersezione e spigolo.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Applica la convalida all'area.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| cell_area | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | L'area.|
| check_intersection | bool | Se controlla l'intersezione di una determinata area con le aree di convalida esistenti.<br/>Se una convalida è stata applicata in una determinata area (o parte di essa),<br/>quindi la convalida esistente dovrebbe essere rimossa in un primo momento da una determinata area.<br/>In caso contrario, potrebbe verificarsi un danneggiamento delle convalide generate.<br/>Se l'utente è sicuro che l'area aggiunta non si interseca con alcuna area esistente,<br/> questo parametro può essere impostato su false per considerazioni sulle prestazioni.|
| check_edge | bool | Se controllare il bordo delle aree applicate di questa convalida.<br/>Le impostazioni interne della convalida dipendono da quella in alto a sinistra dei suoi intervalli applicati,<br/>quindi se una determinata area diventerà la nuova in alto a sinistra degli intervalli applicati,<br/>le impostazioni interne devono essere modificate e ricostruite, altrimenti potrebbero verificarsi risultati imprevisti.<br/>Se l'utente è sicuro che l'area aggiunta non sia quella in alto a sinistra,<br/> questo parametro può essere impostato su false per considerazioni sulle prestazioni.|
###  Osservazioni

In questo metodo, rimuoveremo tutte le vecchie convalide in una determinata area.
Per quello in alto a sinistra degli intervalli applicati di Validation, in primo luogo il suo StartRow è il più piccolo,
in secondo luogo la sua StartColumn è la più piccola di quelle aree che hanno la stessa StartRow più piccola.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Validation](/cells/it/python-net/aspose.cells/validation)
