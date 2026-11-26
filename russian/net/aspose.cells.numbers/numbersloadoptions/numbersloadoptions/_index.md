---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор NumbersLoadOptions. Конструктор"
type: docs
url: /ru/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Конструктор.

```csharp
public NumbersLoadOptions()
```

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать NumbersLoadOptions с помощью конструктора
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Установить некоторые общие свойства
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Сохранить как XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


