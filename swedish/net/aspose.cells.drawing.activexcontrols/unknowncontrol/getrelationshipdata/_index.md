---
title: "UnknownControl.GetRelationshipData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnknownControl-metod. Hämtar den relaterade datan"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/
---
## UnknownControl.GetRelationshipData method

Hämtar den relaterade datan.

```csharp
public byte[] GetRelationshipData(string relId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| relId | String | Relationens id. |

### Returvärde

Returnerar den relaterade datan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlMethodGetRelationshipDataWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Försök att lägga till okänd ActiveX-kontroll
            Shape shape;
            try
            {
                shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 0, 0, 100, 100);
            }
            catch (ArgumentException ex)
            {
                Console.WriteLine($"Could not create control: {ex.Message}");
                return;
            }

            // Hämta kontroll som UnknownControl
            UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
            if (unknownControl == null)
            {
                Console.WriteLine("ActiveX control is not UnknownControl type");
                return;
            }

            try
            {
                // Utför GetRelationshipData med strängparameter
                string relationshipId = "rId1";
                byte[] relationshipData = unknownControl.GetRelationshipData(relationshipId);

                Console.WriteLine("GetRelationshipData executed successfully");
                Console.WriteLine(relationshipData == null 
                    ? "No relationship data found" 
                    : $"Received {relationshipData.Length} bytes of data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("UnknownControlGetRelationshipDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


