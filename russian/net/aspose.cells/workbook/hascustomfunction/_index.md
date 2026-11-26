---
title: "Workbook.HasCustomFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Определяет, используется ли в этой книге пользовательская функция, например в формулах ячеек или в определённых именах"
type: docs
url: /ru/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Определяет, используется ли в этой рабочей книге пользовательская функция, например в формулах ячеек, в определённых именах...

```csharp
public bool HasCustomFunction { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Добавить стандартную формулу к имени
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Добавить пользовательскую функцию к имени
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Тестировать с формулами ячеек
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Стандартная функция в ячейке
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Пользовательская функция в ячейке
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Ссылка на имя с пользовательской функцией
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Комбинированные пользовательские функции
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


