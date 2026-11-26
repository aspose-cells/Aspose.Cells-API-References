---
title: "UnionRange.Hyperlinks"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene todos los hipervínculos en el rango"
type: docs
url: /es/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Obtiene todos los hipervínculos en el rango.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos hipervínculos a las celdas
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Cree un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Obtener hipervínculos en el rango
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Mostrar información sobre cada hipervínculo
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Guarda el libro de trabajo
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


