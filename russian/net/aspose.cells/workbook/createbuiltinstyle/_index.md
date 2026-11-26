---
title: "Workbook.CreateBuiltinStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Создаёт встроенный стиль заданного типа"
type: docs
url: /ru/net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Создаёт встроенный стиль заданного типа.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | BuiltinStyleType | Встроенный стиль типа. |

### Возвращаемое значение

[`Style`](../../style/) object

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateBuiltinStyleWithBuiltinStyleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Применить хороший встроенный стиль
            workbook.Worksheets[0].Cells["A1"].PutValue("Good");
            Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
            workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
            
            // Применить нейтральный встроенный стиль
            workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
            Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
            workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
            
            // Сохраните книгу
            workbook.Save("BuiltinStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


