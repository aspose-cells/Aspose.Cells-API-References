---
title: "Workbook.GetDigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hämtar digital signatur från fil"
type: docs
url: /sv/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Hämtar digital signatur från fil.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Anropa metoden GetDigitalSignature för att hämta digitala signaturer
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Visa information om de digitala signaturerna
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

                // Spara arbetsboken
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

### Se även

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


