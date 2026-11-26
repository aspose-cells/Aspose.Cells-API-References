---
title: "StyleFlag.HorizontalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de alineación horizontal"
type: docs
url: /es/net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Se aplicará la configuración de alineación horizontal.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea datos de ejemplo en celdas
            worksheet.Cells["A1"].PutValue("Left Aligned");
            worksheet.Cells["B1"].PutValue("Center Aligned");
            worksheet.Cells["C1"].PutValue("Right Aligned");
            
            // Crear estilos con diferentes alineaciones horizontales
            Style styleLeft = workbook.CreateStyle();
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            
            Style styleCenter = workbook.CreateStyle();
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            
            Style styleRight = workbook.CreateStyle();
            styleRight.HorizontalAlignment = TextAlignmentType.Right;
            
            // Crear banderas de estilo para aplicar solo la alineación horizontal
            StyleFlag flag = new StyleFlag();
            flag.HorizontalAlignment = true;
            
            // Aplicar estilos a rangos
            Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
            rangeLeft.ApplyStyle(styleLeft, flag);
            
            Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
            rangeCenter.ApplyStyle(styleCenter, flag);
            
            Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
            rangeRight.ApplyStyle(styleRight, flag);
            
            // Guarda el libro de trabajo
            workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


