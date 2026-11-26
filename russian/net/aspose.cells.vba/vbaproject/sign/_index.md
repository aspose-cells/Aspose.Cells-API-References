---
title: "VbaProject.Sign"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProject. Подписать этот VBA проект с помощью DigitalSignature"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/sign/
---
## VbaProject.Sign method

Подписывает этот проект VBA цифровой подписью

```csharp
public void Sign(DigitalSignature digitalSignature)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### Примеры

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodSignWithDigitalSignatureDemo
    {
        public static void Run()
        {
            // Загрузите рабочую книгу с VBA‑проектом
            Workbook workbook = new Workbook("SignXlsm.xlsm");
            
            // Получить VBA проект
            VbaProject vbaProject = workbook.VbaProject;
            
            if (vbaProject != null)
            {
                // Загрузить сертификат из файла
                X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
                
                // Создать цифровую подпись.
                DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
                
                // Подписать VBA проект
                vbaProject.Sign(certSign);
                
                // Сохранить подписанную книгу
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsm);
                    
                    // Проверить подпись
                    Workbook verifyWorkbook = new Workbook(stream);
                    Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
                    Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
                }
            }
        }
    }
}
```

### См. также

* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


