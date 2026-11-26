---
title: "DigitalSignature.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Указывает GUID, который может быть перекрёстно связан с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Empty, все нули Guid"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Empty (все нули) Guid.

```csharp
public Guid Id { get; set; }
```

### Примечания

При установке он связывает [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) с соответствующим [`DigitalSignature`](../).

### Примеры

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте цифровую подпись с определённым ID
            Guid signatureId = Guid.NewGuid();
            
            // Создать цифровую подпись.
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Установите Id подписи
            signature.Id = signatureId;

            // Добавьте подпись в коллекцию
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Примените цифровую подпись к книге
            workbook.SetDigitalSignature(dsCollection);

            // Сохраните книгу
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


