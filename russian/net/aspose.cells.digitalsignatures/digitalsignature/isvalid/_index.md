---
title: "DigitalSignature.IsValid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Если эта цифровая подпись действительна и документ не был изменён, значение будет true"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/isvalid/
---
## DigitalSignature.IsValid property

Если эта цифровая подпись действительна и документ не был изменён, это значение будет true.

```csharp
public bool IsValid { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System.IO;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIsValidDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить некоторые данные в лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Digital Signature");
            
            // Сначала сохраните книгу
            string outputPath = "signed_example.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Создать коллекцию цифровых подписей
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Создайте цифровую подпись (в реальном сценарии используйте правильный сертификат)
            // Первый параметр должен быть byte[] данных сертификата
            byte[] certificateData = File.ReadAllBytes("test.pfx");
            DigitalSignature signature = new DigitalSignature(
                certificateData, 
                "test123", 
                "Test Signature", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Подписать книгу
            workbook.SetDigitalSignature(signatures);
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Проверить подпись
            Workbook signedWorkbook = new Workbook(outputPath);
            DigitalSignatureCollection loadedSignatures = signedWorkbook.GetDigitalSignature();
            
            foreach (DigitalSignature sig in loadedSignatures)
            {
                Console.WriteLine("Signature is valid: " + sig.IsValid);
            }
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


