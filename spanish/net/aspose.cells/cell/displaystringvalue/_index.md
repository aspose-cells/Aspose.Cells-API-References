---
title: "Cell.DisplayStringValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor de cadena formateado de esta celda según el estilo de visualización de la celda"
type: docs
url: /es/net/aspose.cells/cell/displaystringvalue/
---
## Cell.DisplayStringValue property

Obtiene el valor de cadena formateada de esta celda según el estilo de visualización de la celda.

```csharp
public string DisplayStringValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDisplayStringValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cell cell = sheet.Cells[0, 0];
            
            // Primer ejemplo
            Style style = cell.GetStyle();
            style.Custom = "# ##/##\\\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: 3"
            
            // Segundo ejemplo
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3
            
            // Tercer ejemplo
            style.Custom = "\"a\"#\"b\" \"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Cuarto ejemplo con valor decimal
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1b c11d/e47f
            
            // Quinto ejemplo con formato modificado
            style.Custom = "\"a\"#\"b\"\"c\"##\"d\"/\"e\"##\"f\"";
            cell.SetStyle(style);
            cell.PutValue(3);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a3f
            
            // Sexto ejemplo con valor decimal
            cell.PutValue(1.234);
            Console.WriteLine("DisplayStringValue: " + cell.DisplayStringValue); // Output: a1bc11d/e47f
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


