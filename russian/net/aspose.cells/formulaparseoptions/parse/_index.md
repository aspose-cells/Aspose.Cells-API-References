---
title: "FormulaParseOptions.Parse"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaParseOptions. Указывает, следует ли разбирать данную формулу. По умолчанию true. Если false, то строка формулы будет оставаться неизменной в ячейке, пока пользователь не вызовет другие методы для её разбора или пока данные разобранной формулы не потребуются другим операциям, например расчёту формул."
type: docs
url: /ru/net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Разбирать ли данную формулу. По умолчанию true. Если false, то строка формулы будет оставлена как есть в ячейке, пока пользователь не вызовет другие методы для её разбора или пока данные разбора формулы не потребуются другим операциям, например расчёту формул.

```csharp
public bool Parse { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyParseDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить формулы с Parse=false (формулы не будут сразу разбираться)
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["B1"].SetFormula("=A1+A2", new FormulaParseOptions() { Parse = false });
            cells["B2"].SetFormula("=SUM(A1:A2)", new FormulaParseOptions() { Parse = false });

            // Вычислить формулы (разбор произойдёт сейчас)
            wb.CalculateFormula();

            Console.WriteLine("B1 value: " + cells["B1"].Value);
            Console.WriteLine("B2 value: " + cells["B2"].Value);
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


