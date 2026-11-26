---
title: "Cell.FormulaLocal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получить формулу ячейки, отформатированную в локали"
type: docs
url: /ru/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Получить локализованную отформатированную формулу ячейки.

```csharp
public string FormulaLocal { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить локаль по умолчанию на немецкую для демонстрации
            workbook.Settings.Region = CountryCode.Germany;
            
            // Обратиться к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            
            // Установить формулу в стандартном формате (английский)
            cell.Formula = "=SUM(B1:C1)";
            
            // Отобразить формулы как в стандартном, так и в локальном форматах
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Установить формулу в локальном формате (немецкий)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Снова отобразить формулы, чтобы показать разницу
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Продемонстрировать GetFormula с локализацией
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


