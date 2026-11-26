---
title: "Workbook.AddDigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Añade firma digital a un archivo de hoja de cálculo OOXML Excel2007 y posteriores"
type: docs
url: /es/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Agrega una firma digital a un archivo de hoja de cálculo OOXML (Excel2007 y posteriores).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Observaciones

Solo se admite agregar firma digital Xmldsig a un archivo de hoja de cálculo OOXML

### Ejemplos

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos de ejemplo
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Cargar certificado (reemplazar con la ruta y contraseña de su propio certificado)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Crear firma digital
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Crear colección de firmas digitales y agregar firma
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Agregar firma digital al libro de trabajo
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Guarda el libro de trabajo
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Ver también

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


