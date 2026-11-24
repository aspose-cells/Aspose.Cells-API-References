---
title: "NaryEquationNode.LimitLocation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NaryEquationNode Eigenschaft. Dieses Attribut gibt die Position der Grenzen bei n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden"
type: docs
url: /de/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Dieses Attribut gibt die Position der Grenzen bei n-ären Operatoren an. Grenzen können entweder zentriert über und unter dem n-ären Operator liegen oder direkt rechts vom Operator positioniert werden.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um die Gleichung zu enthalten
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Greifen Sie auf die Gleichung zu und fügen Sie einen n-ären Operatorknoten hinzu
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Wandeln Sie zu NaryEquationNode um, um auf LimitLocation zuzugreifen
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Aktuelle LimitLocation anzeigen (Standardwert)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Setze LimitLocation auf SubSup (Grenzen auf der rechten Seite)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Zurück zu UndOvr ändern (zentrierte Grenzen)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


