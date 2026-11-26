---
title: "Класс DigitalSignature"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DigitalSignatures.DigitalSignature. Подпись в файле"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/
---
## DigitalSignature class

Подпись в файле.

```csharp
public class DigitalSignature
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DigitalSignature](digitalsignature/#constructor_1)(X509Certificate2, string, DateTime) | Конструктор digitalSignature. Использует реализацию .Net. |
| [DigitalSignature](digitalsignature/#constructor)(byte[], string, string, DateTime) | Конструктор digitalSignature. Использует реализацию Bouncy Castle. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Certificate](../../aspose.cells.digitalsignatures/digitalsignature/certificate/) { get; set; } | Объект сертификата, использованный для подписи документа. |
| [Comments](../../aspose.cells.digitalsignatures/digitalsignature/comments/) { get; set; } | Назначение подписи. |
| [Id](../../aspose.cells.digitalsignatures/digitalsignature/id/) { get; set; } | Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Empty (все нули) Guid. |
| [Image](../../aspose.cells.digitalsignatures/digitalsignature/image/) { get; set; } | Указывает изображение для цифровой подписи. Значение по умолчанию — null. |
| [IsValid](../../aspose.cells.digitalsignatures/digitalsignature/isvalid/) { get; } | Если эта цифровая подпись действительна и документ не был изменён, это значение будет true. |
| [ProviderId](../../aspose.cells.digitalsignatures/digitalsignature/providerid/) { get; set; } | Указывает идентификатор класса поставщика подписи. Значение по умолчанию — Empty (все нули) Guid. |
| [SignTime](../../aspose.cells.digitalsignatures/digitalsignature/signtime/) { get; set; } | Время, когда документ был подписан. |
| [Text](../../aspose.cells.digitalsignatures/digitalsignature/text/) { get; set; } | Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — Empty. |
| [XAdESType](../../aspose.cells.digitalsignatures/digitalsignature/xadestype/) { get; set; } | Тип XAdES. Значение по умолчанию — None (XAdES отключён). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturesClassDigitalSignatureDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Digital Signature Demo");

            try
            {
                // Создать цифровую подпись с использованием конструктора сертификата
                X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
                DigitalSignature signature = new DigitalSignature(
                    certificate,
                    "Document signed for approval",
                    DateTime.Now);

                // Установить дополнительные свойства
                signature.Id = Guid.NewGuid();
                signature.Text = "Approved";
                signature.XAdESType = XAdESType.XAdES;

                // Добавить подпись в книгу
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                workbook.SetDigitalSignature(signatures);

                // Отобразить информацию о подписи
                Console.WriteLine($"Signature added: {signature.Comments}");
                Console.WriteLine($"Sign time: {signature.SignTime}");
                Console.WriteLine($"Signature ID: {signature.Id}");

                // Сохранить подписанную книгу
                workbook.Save("DigitalSignatureDemo.xlsx");
                Console.WriteLine("Workbook signed and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DigitalSignature: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


