---
title: "PageSetup.PrintTitleColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa las columnas que contienen las celdas que se repiten en el lado izquierdo de cada página"
type: docs
url: /es/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Representa las columnas que contienen las celdas que se repiten en el lado izquierdo de cada página.

```csharp
public string PrintTitleColumns { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la configuración de página
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer columnas de título de impresión para repetir la columna A en cada página impresa
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Agregar algunos datos a la columna A para demostrar el efecto
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


