---
title: "Font.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece el tamaño de la fuente"
type: docs
url: /es/net/aspose.cells/font/size/
---
## Font.Size property

Obtiene o establece el tamaño de la fuente.

```csharp
public int Size { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto con diferentes tamaños de fuente
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // Guarda el libro de trabajo
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


