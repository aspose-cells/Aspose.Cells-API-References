---
title: "PivotItem.GetStringValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItem. Получает строковое значение элемента сводной таблицы. Если значение равно null, будет возвращено"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Получает строковое значение элемента сводки. Если значение равно null, будет возвращена пустая строка ""

```csharp
public string GetStringValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получите доступ к первому листу и сводной таблице
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Получите первое поле строки и его элементы сводной таблицы
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Продемонстрируйте метод GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


