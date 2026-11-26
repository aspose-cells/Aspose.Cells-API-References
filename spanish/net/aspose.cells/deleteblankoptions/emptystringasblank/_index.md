---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteBlankOptions. Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Indica si una celda se considerará en blanco cuando su valor es una cadena vacía. El valor predeterminado es true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar la hoja de cálculo con datos que incluyen cadenas vacías
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Configurar DeleteBlankOptions con EmptyStringAsBlank establecido en true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Eliminar filas que contienen cadenas vacías (tratadas como en blanco)
            worksheet.Cells.DeleteBlankRows(options);

            // Guardar el resultado
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Ver también

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


