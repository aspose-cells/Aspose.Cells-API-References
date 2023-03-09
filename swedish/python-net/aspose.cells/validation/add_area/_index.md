---
title: add_area metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Tillämpar valideringen på området.



```python
def add_area(self, cell_area):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| cell_area | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Området.|
###  Anmärkningar

Det motsvarar att använda [Validation.add_area(cell_area)](/cells/sv/python-net/aspose.cells/validation/add_area)
med kontroll av korsningar och kanter.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Tillämpar valideringen på området.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| cell_area | [CellArea](/cells/sv/python-net/aspose.cells/cellarea) | Området.|
| check_intersection | bool | Om du kontrollerar skärningspunkten mellan ett visst område och befintliga valideringsområden.<br/>Om en validering har tillämpats inom ett visst område (eller en del av det),<br/>då bör den befintliga valideringen först tas bort från ett givet område.<br/>Annars kan korruption orsakas av de genererade valideringarna.<br/>Om användaren är säker på att det tillagda området inte korsar något befintligt område,<br/> Denna parameter kan ställas in som falsk för prestandaövervägande.|
| check_edge | bool | Om du kontrollerar kanten på den här valideringens tillämpade områden.<br/>Valideringens interna inställningar beror på det övre vänstra av dess tillämpade intervall,<br/>så om ett visst område blir det nya övre vänstra av de tillämpade områdena,<br/>de interna inställningarna bör ändras och byggas om, annars kan oväntade resultat orsakas.<br/>Om användaren är säker på att det tillagda området inte är det övre vänstra,<br/> Denna parameter kan ställas in som falsk för prestandaövervägande.|
###  Anmärkningar

I den här metoden tar vi bort alla gamla valideringar inom ett givet område.
För det övre vänstra av Validations tillämpade intervall, för det första är dess StartRow minsta,
för det andra är dess StartColumn den minsta av de områden som har samma minsta StartRow.


###  Se även
* modul [aspose.cells](../../)
* klass [Validation](/cells/sv/python-net/aspose.cells/validation)
