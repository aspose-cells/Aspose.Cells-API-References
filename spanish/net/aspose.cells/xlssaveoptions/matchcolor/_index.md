---
title: "XlsSaveOptions.MatchColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de XlsSaveOptions. Indica si se debe coincidir el color de fuente porque hay 56 colores en la paleta de colores estándar"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Indica si coincidir el color de fuente porque hay 56 colores en la paleta de colores estándar.

```csharp
public bool MatchColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la celda B2 y establecer un texto con un color de fuente específico
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Establecer el color de fuente a azul
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Crear opciones de guardado con MatchColor establecido en true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Guardar el libro de trabajo con las opciones
            workbook.Save("output.xls", saveOptions);

            // Recargar el archivo guardado para verificar que el color se haya preservado
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Verificar que el color de fuente siga siendo azul
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Ver también

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


