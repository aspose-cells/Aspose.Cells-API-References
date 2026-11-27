---
title: "UnknownControl.Data"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnknownControl egenskap. Hämtar och anger den binära datan för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Hämtar och anger den binära datan för kontrollen.

```csharp
public override byte[] Data { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett dummy-CLSID (ogiltig identifierare)
            byte[] dummyClsid = new byte[16];

            // Lägg till en okänd ActiveX-kontroll med ControlType.Unknown med fullständiga parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Åtkomst till UnknownControl-instansen
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Ange kontrollens data inklusive CLSID genom att kopiera in i befintlig array
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Läs och visa information om Data-egenskapen
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Visa hur kontrolldata bevaras i utdatafilen
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


