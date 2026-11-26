---
title: "Workbook.DefaultStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Workbook. Obtiene o establece el objeto Style predeterminado del libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Obtiene o establece el objeto [`Style`](../../style/) predeterminado del libro de trabajo.

```csharp
public Style DefaultStyle { get; set; }
```

### Observaciones

La propiedad DefaultStyle es útil para aplicar un Style a todo el Workbook.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDefaultStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Obtén el style predeterminado y modifica su fuente
            Style defaultStyle = workbook.DefaultStyle;
            defaultStyle.Font.Name = "Tahoma";
            defaultStyle.Font.Size = 12;
            
            // Aplica el style modificado nuevamente como predeterminado
            workbook.DefaultStyle = defaultStyle;
            
            // Crea una hoja de cálculo y agrega texto con el style predeterminado
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This text uses the default Tahoma font");
            
            // Guarda el libro de trabajo
            workbook.Save("DefaultStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


