---
title: "StyleFlag.ShrinkToFit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de encoger para ajustar"
type: docs
url: /es/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

Se aplicará la configuración de reducir para ajustar.

```csharp
public bool ShrinkToFit { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer datos de muestra en una celda
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // Crear un estilo con ShrinkToFit habilitado
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // Crear bandera de estilo y habilitar la bandera ShrinkToFit
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // Aplicar el estilo al rango de celdas (usando explícitamente Aspose.Cells.Range)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // Establecer el ancho de columna para demostrar el encogimiento
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Guarda el libro de trabajo
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


