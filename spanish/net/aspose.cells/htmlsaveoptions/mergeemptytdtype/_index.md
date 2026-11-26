---
title: "HtmlSaveOptions.MergeEmptyTdType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. La opción de combinar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

La opción para fusionar celdas vacías contiguas (elementos td vacíos). El valor predeterminado es MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### Ejemplos

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
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(""); // Empty cell

            // Configurar opciones de guardado HTML con MergeEmptyTdType
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
            {
                MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
            };

            // Guardar en HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, htmlOptions);

            Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
        }
    }
}
```

### Ver también

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


