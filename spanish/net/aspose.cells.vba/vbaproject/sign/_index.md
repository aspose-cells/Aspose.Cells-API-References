---
title: "VbaProject.Sign"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProject. Firma este proyecto VBA con una DigitalSignature"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Firma este proyecto VBA con una DigitalSignature

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Ejemplos

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodSignWithDigitalSignatureDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo con proyecto VBA
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Obtener el proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Cargar certificado desde archivo
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Crear una firma digital
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Firmar el proyecto VBA
                vbaProject.Sign(certSign);
                
                // Guardar el libro de trabajo firmado
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Verificar la firma
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### Ver también

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


