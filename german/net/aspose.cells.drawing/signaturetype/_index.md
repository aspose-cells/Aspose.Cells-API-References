---
title: "Enum SignatureType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.SignatureType Enum. Gibt den Signaturtyp an"
type: docs
url: /de/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Gibt den Signaturtyp an.

```csharp
public enum SignatureType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Der Standardwert, der entsprechende ProviderId-Wert ist fest auf {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | Der entsprechende ProviderId-Wert ist normalerweise {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | Der entsprechende ProviderId-Wert muss normalerweise vom Benutzer festgelegt werden. Er sollte aus der mit dem Anbieter gelieferten Dokumentation entnommen werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Signaturzeilen mit verschiedenen Typen hinzufügen
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Die Arbeitsmappe mit Signaturkonfigurationen speichern
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


