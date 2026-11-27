---
title: "NaryEquationNode.LimitLocation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NaryEquationNode property. Detta attribut specificerar placeringen av gränser i n-ära operatorer. Gränser kan antingen vara centrerade ovanför och under den n-ära operatorn eller placerade precis till höger om operatorn"
type: docs
url: /sv/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Detta attribut anger placeringen av gränser i n-ära operatorer. Gränser kan antingen vara centrerade ovanför och under den n-ära operatorn, eller placerade precis till höger om operatorn.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hålla ekvationen
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Få åtkomst till ekvationen och lägg till en n-är operatornod
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Kasta till NaryEquationNode för att komma åt LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Visa aktuell LimitLocation (standardvärde)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Ställ in LimitLocation till SubSup (gränser på högra sidan)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Ändra tillbaka till UndOvr (centrerade gränser)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Spara arbetsboken
                workbook.Save("LimitLocationDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


