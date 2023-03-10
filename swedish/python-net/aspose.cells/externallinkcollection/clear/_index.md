---
title: clear metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
Tar bort alla externa länkar.



```python
def clear(self):
    ...
```


###  Anmärkningar

När du tar bort externa länkar kommer alla formler som refererar till dem att tas bort också eftersom
referenserna blir ogiltiga.

##  clear(update_references_as_local) {#bool}
Tar bort alla externa länkar.



```python
def clear(self, update_references_as_local):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| update_references_as_local | bool | Om du uppdaterar alla referenser till externa länkar som referenser till själva arbetsboken.|
###  Anmärkningar

Om referenser måste uppdateras kommer referenser till externa länkar i formler att ändras till aktuell arbetsbok.
Till exempel är en cells ursprungliga formel "='externalsource.xlam'!customfunction()",
efter att ha tagit bort externa länkar blir formeln "=customfunction()".
Om referenser inte behöver uppdateras, alla formler med referenser till externa länkar
kommer också att tas bort eftersom dessa referenser blir ogiltiga.


###  Se även
* modul [aspose.cells](../../)
* klass [ExternalLinkCollection](/cells/sv/python-net/aspose.cells/externallinkcollection)
