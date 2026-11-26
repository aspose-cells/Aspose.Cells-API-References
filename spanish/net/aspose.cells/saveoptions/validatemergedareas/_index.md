---
title: "SaveOptions.ValidateMergedAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se deben validar las celdas combinadas antes de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Indica si se validan las celdas combinadas antes de guardar el archivo.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valores y combinar celdas
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // Crear opciones de guardado con ValidateMergedAreas establecido en true
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // Guardar el libro de trabajo con validación de áreas combinadas
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


