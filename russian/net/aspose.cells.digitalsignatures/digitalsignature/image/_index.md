---
title: "DigitalSignature.Image"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Указывает изображение для цифровой подписи. Значение по умолчанию — null"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Указывает изображение для цифровой подписи. Значение по умолчанию — null.

```csharp
public byte[] Image { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.DigitalSignatures;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyImageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Добавьте строку подписи на лист
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Создайте тестовый сертификат (в реальном использовании загрузите из файла)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Создайте цифровую подпись с изображением
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // Добавьте подпись и сохраните
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // Сохранить в поток памяти
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


