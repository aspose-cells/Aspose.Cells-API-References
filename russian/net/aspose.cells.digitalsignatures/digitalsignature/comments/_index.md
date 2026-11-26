---
title: "DigitalSignature.Comments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Предназначение подписи"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/comments/
---
## DigitalSignature.Comments property

Назначение подписи.

```csharp
public string Comments { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyCommentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые образцы данных.
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");

            // Создать цифровую подпись с комментариями
            DigitalSignature signature = new DigitalSignature(
                File.ReadAllBytes("sample.pfx"), 
                "password", 
                "Sample Signature with Comments", 
                DateTime.Now)
            {
                Comments = "This is a test comment for the digital signature"
            };

            // Добавьте подпись в коллекцию
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Подписать книгу
            workbook.SetDigitalSignature(dsCollection);

            // Сохранить подписанную книгу
            string outputPath = "SignedWithComments.xlsx";
            workbook.Save(outputPath);

            // Проверить и отобразить информацию о подписи
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
            }
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


