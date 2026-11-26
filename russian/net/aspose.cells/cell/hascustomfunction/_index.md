---
title: "Cell.HasCustomFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Проверяет, есть ли пользовательская functionunsupported функция в формуле этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Проверяет, есть ли пользовательская функция (неподдерживаемая функция) в формуле этой ячейки.

```csharp
public bool HasCustomFunction { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Добавьте имя пользовательской функции
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Тест с встроенной функцией
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Тест с пользовательской функцией
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Тест с именованным диапазоном, содержащим пользовательскую функцию
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Тест с вложенной пользовательской функцией
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


