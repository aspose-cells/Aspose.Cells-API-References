---
title: "Workbook.GetDigitalSignature"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Gibt die digitale Signatur aus einer Datei zurück"
type: docs
url: /de/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Liest die digitale Signatur aus einer Datei.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Rufen Sie die GetDigitalSignature-Methode auf, um digitale Signaturen abzurufen
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Informationen zu den digitalen Signaturen anzeigen
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


