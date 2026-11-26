---
title: "Workbook.SetDigitalSignature"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Устанавливает цифровую подпись в файл электронной таблицы Excel2007 и более поздних версий"
type: docs
url: /ru/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Устанавливает цифровую подпись в файл таблицы (Excel2007 и новее).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Примечания

Поддерживается только добавление цифровой подписи Xmldsig

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Путь к исходному каталогу
            string sourceDir = "SourceDirectory/";
            
            // Путь к каталогу вывода
            string outputDir = "OutputDirectory/";

            // Загрузить книгу.
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Создайте коллекцию цифровых подписей
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Загрузите файл сертификата
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Создать цифровую подпись
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Добавьте подпись в коллекцию
            digitalSignatures.Add(signature);

            // Установите цифровую подпись в книгу
            workbook.SetDigitalSignature(digitalSignatures);

            // Сохраните книгу
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### См. также

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


