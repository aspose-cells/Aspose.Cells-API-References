---
title: "Workbook.SetDigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del libro de trabajo. Establece una firma digital en un archivo de hoja de cálculo Excel2007 y posteriores"
type: docs
url: /es/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Establece una firma digital en un archivo de hoja de cálculo (Excel2007 y posteriores).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Observaciones

Solo se admite agregar firma digital Xmldsig

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Ruta del directorio de origen
            string sourceDir = "SourceDirectory/";
            
            // Ruta del directorio de salida
            string outputDir = "OutputDirectory/";

            // Cargar el libro de trabajo
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Crear colección de firmas digitales
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Cargar archivo de certificado
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Crear firma digital
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Agregar firma a la colección
            digitalSignatures.Add(signature);

            // Establecer firma digital en el libro de trabajo
            workbook.SetDigitalSignature(digitalSignatures);

            // Guarda el libro de trabajo
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Ver también

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


