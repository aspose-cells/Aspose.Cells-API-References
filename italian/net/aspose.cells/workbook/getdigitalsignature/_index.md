---
title: "Workbook.GetDigitalSignature"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Ottiene la firma digitale dal file"
type: docs
url: /it/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Ottiene la firma digitale dal file.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Chiama il metodo GetDigitalSignature per recuperare le firme digitali
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Visualizza le informazioni sulle firme digitali
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

                // Salva la cartella di lavoro
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

### Vedi anche

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


