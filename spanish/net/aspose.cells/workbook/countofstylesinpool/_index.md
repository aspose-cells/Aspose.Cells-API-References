---
title: "Workbook.CountOfStylesInPool"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene el número de estilos en el pool de estilos"
type: docs
url: /es/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Obtiene el número de estilos en el conjunto de estilos.

```csharp
public int CountOfStylesInPool { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Obtener el recuento inicial de estilos en el pool
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Agregar algunos estilos modificando celdas
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Estilo 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Estilo 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Obtener el recuento actualizado de estilos
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Guardar para demostrar la persistencia de estilos
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


