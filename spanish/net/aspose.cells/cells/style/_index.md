---
title: "Cells.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene y establece el estilo predeterminado de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/style/
---
## Cells.Style property

Obtiene y establece el estilo predeterminado de la hoja de cálculo.

```csharp
public Style Style { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca un valor en la celda A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Obtenga el estilo predeterminado y modifique su formato
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Aplicar el estilo modificado a la celda
            cell.SetStyle(style);

            // Muestre el valor de cadena formateado
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


