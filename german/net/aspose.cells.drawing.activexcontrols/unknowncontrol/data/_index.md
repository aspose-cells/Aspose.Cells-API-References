---
title: "UnknownControl.Data"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnknownControl-Eigenschaft. Ruft die Binärdaten des Steuerelements ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Liest und setzt die Binärdaten des Steuerelements.

```csharp
public override byte[] Data { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Dummy-CLSID (ungültiger Bezeichner)
            byte[] dummyClsid = new byte[16];

            // Füge ein unbekanntes ActiveX-Steuerelement mit ControlType.Unknown und vollständigen Parametern hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Greife auf die UnknownControl-Instanz zu
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Setze die Daten des Steuerelements einschließlich CLSID, indem du sie in ein vorhandenes Array kopierst
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Lese und zeige Informationen der Data-Eigenschaft an
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Demonstrieren Sie die Persistenz von Steuerungsdaten in der Ausgabedatei
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


