---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldGroupOptions. Получает или задает тип группировки для сводного поля. Только для группировки полей даты и времени."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Получает или задает тип группировки для поля сводной таблицы. Только для группировки поля даты и времени.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Примеры

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Группировать по году и месяцу вместе
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### См. также

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


