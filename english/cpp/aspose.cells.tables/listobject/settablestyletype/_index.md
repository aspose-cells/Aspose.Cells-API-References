---
title: Aspose::Cells::Tables::ListObject::SetTableStyleType method
linktitle: SetTableStyleType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Tables::ListObject::SetTableStyleType method. Gets and the built-in table style in C++.'
type: docs
weight: 4200
url: /cpp/aspose.cells.tables/listobject/settablestyletype/
---
## ListObject::SetTableStyleType method


Gets and the built-in table style.

```cpp
void Aspose::Cells::Tables::ListObject::SetTableStyleType(TableStyleType value)
```


## Examples


```cpp
Aspose::Cells::Startup();
Workbook workbook(u"Book1.xlsx");
ListObjectCollection tables = workbook.GetWorksheets().Get(0).GetListObjects();
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables.Get(0);
if(table.GetTableStyleType() != TableStyleType::TableStyleDark2)
{
    table.SetTableStyleType(TableStyleType::TableStyleDark2);
}
workbook.Save(u"TableStyle.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Enum [TableStyleType](../../tablestyletype/)
* Class [ListObject](../)
* Namespace [Aspose::Cells::Tables](../../)
* Library [Aspose.Cells for C++](../../../)
