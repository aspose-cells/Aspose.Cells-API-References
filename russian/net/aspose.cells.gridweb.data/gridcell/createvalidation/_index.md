---
title: "GridCell.CreateValidation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridCell. Создает объект проверки для ячейки"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Создаёт объект проверки для ячейки.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| validationType | GridValidationType | Тип проверки. |
| isRequried | Boolean | Указывает, требуется ли значение ячейки. |

### Примеры

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Устанавливает числовое выражение проверки.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### См. также

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


