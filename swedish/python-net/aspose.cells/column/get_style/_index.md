---
title: get_style metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells/column/get_style/
is_root: false
---
##  get_style() {#}
Får stilen i denna kolumn.



```python
def get_style(self):
    ...
```


###  Anmärkningar

Att ändra det returnerade stilobjektet direkt får ingen effekt för den här kolumnen eller några celler i den här kolumnen.
Du måste ringa [Column.apply_style(style, flag)](/cells/sv/python-net/aspose.cells/column/apply_style) eller [Column.set_style(style)](/cells/sv/python-net/aspose.cells/column/set_style) metod
för att tillämpa ändringen på den här kolumnen.

Kolumnens stil är stilen som kommer att ärvas av celler i den här kolumnen (de celler som inte har några anpassade stilinställningar,
såsom befintliga celler som inte har ställts in stil uttryckligen, eller de som inte har instansierats)


###  Se även
* modul [aspose.cells](../../)
* klass [Column](/cells/sv/python-net/aspose.cells/column)
