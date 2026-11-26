---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de pagesetup será inválido y los demás ajustes de pagesetup seguirán aplicándose."
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Agregar algunos datos de muestra a ambas hojas
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // Establecer opciones de guardado PDF con OnePagePerSheet
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Guarda el libro de trabajo en PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


