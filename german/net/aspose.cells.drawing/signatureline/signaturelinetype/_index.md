---
title: "SignatureLine.SignatureLineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SignatureLine-Eigenschaft. Gibt den Signaturtyp zurück oder legt ihn fest. Default  Wenn der Standardwert gesetzt ist, ist der entsprechende ProviderId-Wert fest auf 00000000000000000000000000000000. Stamp  Wenn der Wert Stamp ist, ist der entsprechende ProviderId-Wert normalerweise 000CD6A400000000C000000000000046. Custom  Wenn der Wert Custom ist, muss der entsprechende ProviderId-Wert in der Regel vom Benutzer festgelegt werden. Er sollte aus der Dokumentation des Anbieters entnommen werden."
type: docs
url: /de/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Ruft den Signaturtyp ab oder legt ihn fest. Default - Wenn der Standardwert festgelegt ist, ist der entsprechende ProviderId-Wert auf {0000000000-0000-0000-0000-0000000000} fixiert. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId-Wert normalerweise {000CD6A4-0000-0000-C000-000000000046}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId-Wert in der Regel vom Benutzer festgelegt werden. Er sollte aus der mit dem Provider gelieferten Dokumentation entnommen werden.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Signaturzeile
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Zeige den aktuellen SignatureLineType an
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Setze SignatureLineType auf Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Füge die Signaturzeile dem Arbeitsblatt hinzu, indem du sie zu den Formen hinzufügst
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Ändere SignatureLineType zu Custom mit benutzerdefinierter ProviderId
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Speichere die Arbeitsmappe
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


