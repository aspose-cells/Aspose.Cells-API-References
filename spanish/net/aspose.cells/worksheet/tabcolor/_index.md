---
title: "Worksheet.TabColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Representa el color de la pestaña de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Representa el color de la pestaña de la hoja.

```csharp
public Color TabColor { get; set; }
```

### Observaciones

Esta característica solo es compatible con ExcelXP (Excel2002) y versiones posteriores. Si guarda el archivo en formato Excel97 o Excel2000, se omitirá.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el color de la pestaña a rojo
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Borrar el color de la pestaña
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Guardar el libro de trabajo modificado
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


