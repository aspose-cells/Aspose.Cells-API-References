---
title: "Hyperlink.Area"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Hyperlink. Obtiene el rango del hipervínculo"
type: docs
url: /es/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Obtiene el rango del hipervínculo.

```csharp
public CellArea Area { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // Agregar hipervínculos
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // Acceder a los hipervínculos y demostrar el uso de la propiedad Area
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // Verificar si el hipervínculo está en la celda A4 usando la propiedad Area
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


