---
title: "DigitalSignatureCollection.DigitalSignatureCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DigitalSignatureCollection. Конструктор класса DigitalSignatureCollection"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignaturecollection/digitalsignaturecollection/
---
## DigitalSignatureCollection constructor

Конструктор класса DigitalSignatureCollection.

```csharp
public DigitalSignatureCollection()
```

### Примеры

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureCollectionMethodCtorDemo
    {
        public static void Run()
        {
            // Инициализируйте новую DigitalSignatureCollection
            DigitalSignatureCollection certSigns = new DigitalSignatureCollection();

            // Загрузите сертификат и создайте цифровую подпись
            string pfx = "ForTest.pfx";
            string password = "123456";
            string comment = "test";
            
            X509Certificate2 cert = new X509Certificate2(pfx, password);
            DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
            
            // Добавьте подпись в коллекцию
            certSigns.Add(certSign);

            Console.WriteLine("Digital signature collection created with 1 signature.");
        }
    }
}
```

### См. также

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


