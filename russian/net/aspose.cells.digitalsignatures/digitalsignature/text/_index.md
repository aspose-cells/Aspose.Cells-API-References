---
title: "DigitalSignature.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — Empty"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/text/
---
## DigitalSignature.Text property

Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — Empty.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте тестовый сертификат (в реальном сценарии используйте действительный сертификат)
            X509Certificate2 certificate = null;
            try
            {
                certificate = new X509Certificate2();
            }
            catch
            {
                Console.WriteLine("Could not create certificate. Using null for demonstration.");
            }

            // Создайте экземпляр цифровой подписи
            DigitalSignature signature = new DigitalSignature(
                certificate,
                "Sample signature comments",
                DateTime.Now);

            // Отобразите текущее значение Text (по умолчанию пусто)
            Console.WriteLine("Current Text value: " + signature.Text);

            // Установите новое значение свойства Text
            signature.Text = "Approved by John Doe";

            // Создайте коллекцию цифровых подписей и добавьте в неё подпись
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            signatures.Add(signature);

            // Добавьте цифровые подписи в рабочую книгу
            workbook.AddDigitalSignature(signatures);

            // Сохраните книгу с цифровой подписью
            try
            {
                workbook.Save("DigitalSignatureWithText.xlsx");
                Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error saving workbook: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


