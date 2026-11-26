---
title: "HtmlSaveOptions.MergeEmptyTdType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Параметр для объединения смежных пустых ячеек (empty td elements). Значение по умолчанию — MergeEmptyTdType.Default"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

Опция объединения смежных пустых ячеек (пустых элементов td). Значение по умолчанию — MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(""); // Empty cell

            // Настроить параметры сохранения HTML с MergeEmptyTdType
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
            {
                MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
            };

            // Сохранить в HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, htmlOptions);

            Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
        }
    }
}
```

### См. также

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


