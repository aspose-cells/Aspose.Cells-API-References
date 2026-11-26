---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Создаёт объект Range из адреса диапазона"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Создаёт объект [`Range`](../../range/) из адреса диапазона.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| address | String | Адрес диапазона. |
| sheetIndex | Int32 | Индекс листа. |

### Возвращаемое значение

Объект [`Range`](../../range/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать объединённый диапазон из строк адресов
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Установить значение для всего объединённого диапазона
            unionRange.Value = "Test";
            
            // Применить стиль к объединённому диапазону
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Сохраните книгу
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


