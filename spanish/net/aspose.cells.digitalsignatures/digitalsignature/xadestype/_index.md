---
title: "DigitalSignature.XAdESType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Tipo XAdES. El valor predeterminado es None. XAdES está desactivado"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/xadestype/
---
## DigitalSignature.XAdESType property

Tipo XAdES. El valor predeterminado es None (XAdES está desactivado).

```csharp
public XAdESType XAdESType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyXAdESTypeDemo
    {
        public static void Run()
        {
            string pfxPath = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            string sourceFile = "example.xlsx";
            string outputFile = "signed_example.xlsx";

            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, comment, DateTime.Now);
            signature.XAdESType = XAdESType.XAdES;
            signatures.Add(signature);

            Workbook workbook = new Workbook(sourceFile);
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputFile);
        }
    }
}
```

### Ver también

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


