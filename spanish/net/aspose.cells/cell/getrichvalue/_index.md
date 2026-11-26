---
title: "Cell.GetRichValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el valor enriquecido de la celda"
type: docs
url: /es/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Obtiene el valor enriquecido de la celda.

```csharp
public CellRichValue GetRichValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet ws = wb.Worksheets[0];
            
            // Establezca un valor de texto enriquecido en la celda A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Obtener el valor enriquecido de la celda A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Muestre el valor de texto enriquecido
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Guarda el libro de trabajo
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


