---
title: "DigitalSignature.XAdESType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Тип XAdES. Значение по умолчанию — None, XAdES отключён"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/xadestype/
---
## DigitalSignature.XAdESType property

Тип XAdES. Значение по умолчанию — None (XAdES отключён).

```csharp
public XAdESType XAdESType { get; set; }
```

### Примеры

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

### См. также

* enum [XAdESType](../../xadestype/)
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


