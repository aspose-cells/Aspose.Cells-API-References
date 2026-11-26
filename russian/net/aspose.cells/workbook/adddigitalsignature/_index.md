---
title: "Workbook.AddDigitalSignature"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Добавляет цифровую подпись в файл электронной таблицы OOXML Excel2007 и более поздних версий"
type: docs
url: /ru/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Добавляет цифровую подпись в файл электронных таблиц OOXML (Excel2007 и новее).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Примечания

Поддерживается только добавление цифровой подписи Xmldsig в файл электронной таблицы OOXML

### Примеры

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые образцы данных.
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Загрузить сертификат (замените на свой путь к сертификату и пароль)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Создать цифровую подпись
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Создать коллекцию цифровых подписей и добавить подпись
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Добавить цифровую подпись в рабочую книгу
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Сохраните книгу
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### См. также

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


