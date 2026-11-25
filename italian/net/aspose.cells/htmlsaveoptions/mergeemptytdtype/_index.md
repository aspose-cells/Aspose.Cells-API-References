---
title: "HtmlSaveOptions.MergeEmptyTdType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(""); // Empty cell

            // Configura le opzioni di salvataggio HTML con MergeEmptyTdType
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
            {
                MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
            };

            // Salva in HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, htmlOptions);

            Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
        }
    }
}
```

### Vedi anche

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


