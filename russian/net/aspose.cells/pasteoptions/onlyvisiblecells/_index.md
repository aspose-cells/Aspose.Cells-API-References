---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. True означает копирование только видимых ячеек"
type: docs
url: /ru/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True означает копирование только видимых ячеек.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Создать книгу с двумя листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Получить ячейки с первого листа и заполнить данными
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Скрыть некоторые строки и столбцы
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Создать исходный диапазон для копирования
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Получить ячейки со второго листа для назначения
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Создать параметры вставки и установить OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Копировать только видимые ячейки
            destRange.Copy(sourceRange, pasteOptions);
            
            // Вывести результаты для демонстрации функциональности
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### См. также

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


