---
title: "Cell.GetHtmlString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene la cadena html que contiene datos y algunos formatos en esta celda"
type: docs
url: /es/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Obtiene la cadena HTML que contiene datos y algunos formatos en esta celda.

```csharp
public string GetHtmlString(bool html5)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| html5 | Booleano | Indica si el valor es compatible con html5 |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer un valor de celda de ejemplo con formato
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Demostrar GetHtmlString con un parámetro booleano
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


