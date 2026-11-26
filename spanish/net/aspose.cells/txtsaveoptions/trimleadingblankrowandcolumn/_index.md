---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace ms excel. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Indica si las filas y columnas en blanco iniciales deben recortarse como lo hace MS Excel. El valor predeterminado es verdadero.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Observaciones

Lo mismo con la regla en ms excel, una fila/columna no se considerará en blanco si tiene un estilo personalizado, incluso si no contiene datos de celda. Al guardar en modo LightCells, esta opción no tiene efecto. El usuario debe controlar el rango de salida mediante la implementación de [`LightCellsDataProvider`](../lightcellsdataprovider/) o especificando [`ExportArea`](../exportarea/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con algunos datos y filas/columnas en blanco
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos con filas/columnas en blanco iniciales
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Guardar sin recortar los espacios en blanco iniciales
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Guardar recortando los espacios en blanco iniciales
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


