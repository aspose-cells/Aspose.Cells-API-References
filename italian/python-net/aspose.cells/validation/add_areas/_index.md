---
title: metodo add_areas
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/validation/add_areas/
is_root: false
---
##  add_areas(areas, check_intersection, check_edge) {#list-bool-bool}
Applica la convalida a determinate aree.



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| areas | list | Le zone.|
| check_intersection | bool | Se controlla l'intersezione di una determinata area con le aree di convalida esistenti.<br/>Se una convalida è stata applicata in una determinata area (o parte di essa),<br/>quindi la convalida esistente dovrebbe essere rimossa in un primo momento da una determinata area.<br/>In caso contrario, potrebbe verificarsi un danneggiamento delle convalide generate.<br/>Se l'utente è sicuro che tutte le aree aggiunte non si intersecano con nessuna area esistente,<br/> questo parametro può essere impostato su false per considerazioni sulle prestazioni.|
| check_edge | bool | Se controllare il bordo delle aree applicate di questa convalida.<br/>Le impostazioni interne della convalida dipendono da quella in alto a sinistra dei suoi intervalli applicati,<br/>quindi se una delle aree date diventerà la nuova in alto a sinistra degli intervalli applicati,<br/>le impostazioni interne devono essere modificate e ricostruite, altrimenti potrebbero verificarsi risultati imprevisti.<br/>Se l'utente è sicuro che nessuna di queste aree aggiunte sia in alto a sinistra,<br/> questo parametro può essere impostato su false per considerazioni sulle prestazioni.|
###  Osservazioni

In questo metodo, rimuoveremo tutte le vecchie convalide in una determinata area.
Per quello in alto a sinistra degli intervalli applicati di Validation, in primo luogo il suo StartRow è il più piccolo,
in secondo luogo la sua StartColumn è la più piccola di quelle aree che hanno la stessa StartRow più piccola.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Validation](/cells/it/python-net/aspose.cells/validation)
