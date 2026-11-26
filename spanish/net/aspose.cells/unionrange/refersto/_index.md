---
title: "UnionRange.RefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene a qué se refieren los rangos"
type: docs
url: /es/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Obtiene a qué se refiere el rango.

```csharp
public string RefersTo { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Crear un rango con nombre
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Crear un rango de unión que incluya nuestro rango con nombre
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Mostrar la propiedad RefersTo del rango de unión
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Crear otro rango y mostrar su RefersTo
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Demostrar el uso de RefersTo para identificar la composición del rango
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Mostrar cómo cambia RefersTo cuando se modifican los rangos
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Guarda el libro de trabajo
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


