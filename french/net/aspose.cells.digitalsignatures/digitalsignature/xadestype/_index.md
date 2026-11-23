---
title: "DigitalSignature.XAdESType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DigitalSignature. Type XAdES. La valeur par défaut est None (XAdES désactivé)"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignature/xadestype/
---
## DigitalSignature.XAdESType property

Type XAdES. La valeur par défaut est None (XAdES est désactivé).

```csharp
public XAdESType XAdESType { get; set; }
```

### Exemples

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

### Voir aussi

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


