---
title: "CalculationOptions.LinkedDataSources"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает источники данных для внешних ссылок, используемых в формулах"
type: docs
url: /ru/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Указывает источники данных для внешних ссылок, используемых в формулах.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Примечания

Как и в случае [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), здесь вы можете указать источники данных для внешних ссылок, используемых в формулах, которые будут вычисляться, особенно для тех, которые применяются в функции INDIRECT. Для внешних ссылок, используемых в функции INDIRECT, они не считаются частью внешних ссылок книги и не могут быть обновлены с помощью [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). Соответствие этих книг с внешними ссылками определяется по [`FileName`](../../workbook/filename/) и [`DataSource`](../../externallink/datasource/). Поэтому убедитесь, что у [`FileName`](../../workbook/filename/) указано правильное значение (обычно оно должно совпадать с соответствующим [`DataSource`](../../externallink/datasource/)) для каждой книги, чтобы они могли быть связаны как ожидается.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Создайте внешнюю книгу с данными
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Добавьте именованные диапазоны во внешнюю книгу
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Создайте основную книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Установите формулы, ссылающиеся на внешнюю книгу
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Вычислите формулы, используя LinkedDataSources
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


