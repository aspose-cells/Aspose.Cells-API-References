---
title: "DigitalSignature.SignTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Время, когда документ был подписан"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/signtime/
---
## DigitalSignature.SignTime property

Время, когда документ был подписан.

```csharp
public DateTime SignTime { get; set; }
```

### Примеры

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertySignTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");

            // Создайте и добавьте цифровую подпись
            try
            {
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
                
                DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
                dsc.Add(signature);

                // Продемонстрируйте свойство SignTime
                Console.WriteLine("Signature added at: " + signature.SignTime);

                // Сохранить подписанную книгу
                workbook.Save("SignedWorkbook.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


