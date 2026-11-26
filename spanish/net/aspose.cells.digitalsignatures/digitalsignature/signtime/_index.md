---
title: "DigitalSignature.SignTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. El tiempo en que el documento fue firmado"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

La hora en que se firmó el documento.

```csharp
public DateTime SignTime { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertySignTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // Crear y agregar una firma digital
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // Demostrar la propiedad SignTime
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // Guardar el libro de trabajo firmado
                workbook.Save("SignedWorkbook.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


