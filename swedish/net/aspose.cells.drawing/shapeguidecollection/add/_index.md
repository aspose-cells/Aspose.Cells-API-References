---
title: "ShapeGuideCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeGuideCollection-metod. Lägger till en formguide. Viktigt: Denna funktion är för närvarande endast tillgänglig för Excel07 och senare"
type: docs
url: /sv/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Lägger till en formguide. (Viktigt: Denna funktion är för närvarande endast tillgänglig för Excel07 och senare)

```csharp
public int Add(string name, double val)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | namnet på justering. Det är som "adj(Används när det bara finns ett justeringsvärde)", "adj1", "adj2", "adj3" och så vidare. |
| val | Double | värdet på justering |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form som använder justeringsguider
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Hämta ShapeGuideCollection från formens geometrijusteringar
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Anropa Add-metoden med parametrarna (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


