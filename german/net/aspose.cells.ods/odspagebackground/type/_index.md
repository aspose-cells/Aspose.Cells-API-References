---
title: "OdsPageBackground.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsPageBackground-Eigenschaft. Gibt den Seitentyp des Hintergrunds zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Liest und setzt den Seitenhintergrundtyp.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf die Seiteneinrichtung des ersten Arbeitsblatts
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Den ODS-Seitenhintergrund abrufen
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Hintergrundtyp auf Grafik setzen und konfigurieren
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.ods");
            
            // Die gespeicherte Datei neu laden, um die Einstellungen zu überprüfen
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Die Überprüfungsergebnisse ausgeben
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Siehe auch

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


