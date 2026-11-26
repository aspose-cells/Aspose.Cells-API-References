---
title: "PasteOptions.PasteType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. Тип специальной вставки"
type: docs
url: /ru/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Тип специальной вставки.

```csharp
public PasteType PasteType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить значение источника
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Создать диапазоны с полностью квалифицированными именами типов
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Копировать с PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Вывести результаты
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### См. также

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


