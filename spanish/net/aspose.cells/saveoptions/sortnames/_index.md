---
title: "SaveOptions.SortNames"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se ordenan los nombres definidos antes de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Indica si se ordenan los nombres definidos antes de guardar el archivo.

```csharp
public bool SortNames { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Crea un nuevo objeto Workbook
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crear un rango con nombre
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Crear opciones de guardado con SortNames habilitado
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Guarda el libro de trabajo
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


