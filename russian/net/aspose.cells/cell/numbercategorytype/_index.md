---
title: "Cell.NumberCategoryType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Представляет тип категории числового форматирования этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Представляет тип категории числового форматирования этой ячейки.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Примечания

Когда шаблон форматирования ячейки комбинируется с шаблонами условного форматирования, возвращаемый тип соответствует части, используемой для текущего значения этой ячейки. Например, если шаблон форматирования этой ячейки — "#,##0;(#,##0);"-";@", то когда значение ячейки числовое и не равно 0, возвращаемый тип — Number; когда значение ячейки равно 0 или не является числом, возвращаемый тип — Text.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте значение даты в ячейку A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Установите формат даты
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Добавьте числовое значение в ячейку A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Добавьте текстовое значение в ячейку A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Отобразите NumberCategoryType для каждой ячейки
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Измените формат A2 на валютный и проверьте NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### См. также

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


