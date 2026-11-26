---
title: "Cell.IsTableFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли эта ячейка частью табличной формулы"
type: docs
url: /ru/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Указывает, является ли эта ячейка частью формулы таблицы.

```csharp
public bool IsTableFormula { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать таблицу
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Добавить табличную формулу в ячейку D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Проверьте, содержит ли ячейка табличную формулу
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


