---
title: "DigitalSignature.DigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de DigitalSignature. Constructor de digitalSignature. Utiliza la implementación .Net"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Constructor de digitalSignature. Utiliza la implementación de .Net.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| certificado | X509Certificate2 | Objeto de certificado que se utilizó para firmar el documento. |
| comentarios | String | El propósito de la firma. |
| signTime | DateTime | La hora UTC cuando se firmó el documento. |

### Ejemplos

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // Crear una colección de firmas digitales
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Cargar certificado con clave privada
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Crear firma digital con certificado, propósito y marca de tiempo
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Crear un nuevo libro de trabajo y firmarlo
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Constructor de digitalSignature. Utiliza la implementación de Bouncy Castle.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rawData | Byte[] | Una matriz de bytes que contiene datos de un certificado X.509. |
| contraseña | String | La contraseña requerida para acceder a los datos del certificado X.509. |
| comentarios | String | El propósito de la firma. |
| signTime | DateTime | La hora UTC cuando se firmó el documento. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar contenido de ejemplo
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Cargar archivo de certificado como matriz de bytes (reemplazar con la ruta real del certificado)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Crear parámetros de firma digital
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Llamar al constructor con (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Crear una DigitalSignatureCollection y agregar la firma a ella
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Agregar firmas al libro de trabajo
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


