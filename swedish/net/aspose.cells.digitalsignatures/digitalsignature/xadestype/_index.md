---
title: "DigitalSignature.XAdESType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. XAdES-typ. Standardvärdet är None. XAdES är avstängt."
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/xadestype/
---
## DigitalSignature.XAdESType property

XAdES-typ. Standardvärdet är None (XAdES är avstängt).

```csharp
public XAdESType XAdESType { get; set; }
```

### Exempel

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

### Se även

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


