---
title: "DigitalSignature.DigitalSignature"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DigitalSignature. Конструктор digitalSignature. Использует реализацию .Net"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/digitalsignature/
---
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}

Конструктор digitalSignature. Использует реализацию .Net.

```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| сертификат | X509Certificate2 | Объект сертификата, использованный для подписи документа. |
| комментарии | String | Назначение подписи. |
| signTime | DateTime | Время UTC, когда документ был подписан. |

### Примеры

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
    {
        public static void Run()
        {
            // Создать коллекцию цифровых подписей
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();
            
            // Загрузить сертификат с закрытым ключом
            X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
            
            // Создать цифровую подпись с сертификатом, назначением и меткой времени
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Document approval", 
                DateTime.Now);
                
            signatures.Add(signature);
            
            // Создать новую книгу и подписать её
            Workbook workbook = new Workbook();
            workbook.SetDigitalSignature(signatures);
            workbook.Save("signed_document.xlsx");
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)

---

## DigitalSignature(byte[], string, string, DateTime) {#constructor}

Конструктор digitalSignature. Использует реализацию Bouncy Castle.

```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rawData | Byte[] | Массив байтов, содержащий данные из сертификата X.509. |
| пароль | String | Пароль, необходимый для доступа к данным сертификата X.509. |
| комментарии | String | Назначение подписи. |
| signTime | DateTime | Время UTC, когда документ был подписан. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;

    public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерное содержимое
            worksheet.Cells["A1"].PutValue("Digitally Signed Document");
            
            try
            {
                // Загрузить файл сертификата как массив байтов (заменить реальным путём к сертификату)
                string certPath = "certificate.pfx";
                byte[] certData = File.ReadAllBytes(certPath);
                
                // Создать параметры цифровой подписи
                string password = "certificate_password";
                string comments = "Approved by John Doe";
                DateTime signTime = DateTime.Now;
                
                // Вызвать конструктор с (Byte[], String, String, DateTime)
                DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
                
                // Создать DigitalSignatureCollection и добавить в неё подпись
                DigitalSignatureCollection signatures = new DigitalSignatureCollection();
                signatures.Add(signature);
                
                // Добавить подписи в книгу
                workbook.AddDigitalSignature(signatures);
                
                Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("DigitalSignatureDemo.xlsx");
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


