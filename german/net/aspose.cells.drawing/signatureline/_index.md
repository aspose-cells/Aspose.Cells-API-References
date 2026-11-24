---
title: "Klasse SignatureLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.SignatureLine Klasse. Stellt die Signaturzeile dar"
type: docs
url: /de/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Stellt die Signaturzeile dar.

```csharp
public class SignatureLine
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SignatureLine](signatureline/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Gibt an, ob Kommentare angehängt werden können. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Liest oder setzt die E‑Mail des Unterzeichners. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Liest oder setzt den Bezeichner für diese Signaturzeile. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Liest oder setzt den Text, der dem Benutzer zur Signaturzeit angezeigt wird. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Gibt an, ob es sich um eine Signaturzeile handelt. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Liest oder setzt die ID des Signaturanbieters. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Gibt an, ob das Signaturdatum angezeigt wird. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Ruft den Signaturtyp ab oder legt ihn fest. Default - Wenn der Standardwert festgelegt ist, ist der entsprechende ProviderId-Wert auf {0000000000-0000-0000-0000-0000000000} fixiert. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId-Wert normalerweise {000CD6A4-0000-0000-C000-000000000046}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId-Wert in der Regel vom Benutzer festgelegt werden. Er sollte aus der mit dem Provider gelieferten Dokumentation entnommen werden. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Ruft den Unterzeichner ab oder legt ihn fest. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Ruft den Titel des Sängers ab oder legt ihn fest. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Bild hinzufügen
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Erstelle Signaturzeilenobjekt
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Weisen Sie das Signaturzeilenobjekt der Eigenschaft Picture.SignatureLine zu
            pic.SignatureLine = s;

            // Speichere die Excel-Datei
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


