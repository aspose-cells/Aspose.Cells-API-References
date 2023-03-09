---
title: get_style metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells/row/get_style/
is_root: false
---
##  get_style() {#}
Får stilen på den här raden.



```python
def get_style(self):
    ...
```


###  Anmärkningar

Att ändra det returnerade stilobjektet direkt får ingen effekt för den här raden eller några celler i den här raden.
Du måste ringa [Row.apply_style(style, flag)](/cells/sv/python-net/aspose.cells/row/apply_style) eller [Row.set_style(style)](/cells/sv/python-net/aspose.cells/row/set_style) metod
för att tillämpa ändringen på den här raden.

Radens stil är stilen som kommer att ärvas av celler i den här raden (de celler som inte har några anpassade stilinställningar,
såsom befintliga celler som inte har ställts in stil uttryckligen, eller de som inte har instansierats)


###  Se även
* modul [aspose.cells](../../)
* klass [Row](/cells/sv/python-net/aspose.cells/row)
