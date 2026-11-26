---
title: "Name.SheetIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Name. Указывает, что это имя принадлежит Workbook или Worksheet. 0  Глобальное имя, иначе индекс листа, начиная с 1"
type: docs
url: /ru/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Указывает, принадлежит ли это имя книге Workbook или листу Worksheet. 0 = глобальное имя, иначе индекс листа (нумерация с единицы).

```csharp
public int SheetIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Создать именованный диапазон в Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Отобразить индекс листа именованного диапазона
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Сохраните книгу
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


