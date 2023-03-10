---
title: remove_at metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
Tar bort den angivna externa länken från arbetsboken.



```python
def remove_at(self, index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| index | int | indexet för den externa länken som ska tas bort.|
###  Anmärkningar

När du tar bort den externa länken kommer alla formler som refererar till den att tas bort också eftersom
referenserna blir ogiltiga.

##  remove_at(index, update_references_as_local) {#int-bool}
Tar bort den angivna externa länken från arbetsboken.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| index | int | indexet för den externa länken som ska tas bort.|
| update_references_as_local | bool | Om du uppdaterar alla referenser för given extern länk till referens till den aktuella arbetsboken själv.|
###  Anmärkningar

Om referenser måste uppdateras kommer referenser till externa länkar i formler att ändras till aktuell arbetsbok.
Till exempel är den externa länken som ska tas bort "externalsource.xlam" och den definierar en anpassad funktion "customfunction()",
en cells ursprungliga formel är "='externalsource.xlam'!customfunction()",
efter att ha tagit bort formeln blir "=customfunction()".
Om referensen inte behöver uppdateras, alla formler med hänvisning till denna externa länk
kommer också att tas bort eftersom dessa referenser blir ogiltiga.


###  Se även
* modul [aspose.cells](../../)
* klass [ExternalLinkCollection](/cells/sv/python-net/aspose.cells/externallinkcollection)
