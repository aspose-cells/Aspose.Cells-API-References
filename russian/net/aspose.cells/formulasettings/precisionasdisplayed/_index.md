---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaSettings. Указывает, должна ли точность вычисленного результата устанавливаться в соответствии с отображаемым значением при вычислении формул"
type: docs
url: /ru/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Указывает, должна ли точность вычисленного результата устанавливаться в соответствии с отображением при вычислении формул.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Установить PrecisionAsDisplayed в значение true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Установить формат отображения для ячейки A1, чтобы показывать 2 десятичных знака
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Установить формулу в ячейке B1, которая ссылается на A1
            cells["B1"].Formula = "=A1";
            
            // Вычислить формулы с включённым PrecisionAsDisplayed
            workbook.CalculateFormula();
            
            // Вывести результаты
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### См. также

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


