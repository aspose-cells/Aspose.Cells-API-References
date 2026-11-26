---
title: "PivotField.OriginalItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Получить исходные базовые элементы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Получить оригинальные базовые элементы;

```csharp
public string[] OriginalItems { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Получить доступ к первому полю строки
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Отобразить исходные элементы и сгруппированные элементы
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Сохранить изменённую книгу
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


