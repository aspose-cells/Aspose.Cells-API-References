---
title: "Cell.IsCheckBoxStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Указывает, является ли данная ячейка флажком"
type: docs
url: /ru/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Указывает, можно ли установить эту ячейку как флажок.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получите доступ к ячейке B1 и установите её в стиль флажка
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Получите доступ к ячейке A1 и установите её в стиль флажка со значением
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Сохраните книгу
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Проверьте, что B1 имеет стиль флажка
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // Измените B1 на стиль без флажка и сохраните
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


