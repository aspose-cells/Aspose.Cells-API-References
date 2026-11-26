---
title: "VbaProject.CertRawData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProject. Получает необработанные данные сертификата, если этот VBA проект подписан"
type: docs
url: /ru/net/aspose.cells.vba/vbaproject/certrawdata/
---
## VbaProject.CertRawData property

Получает необработанные данные сертификата, если этот VBA‑проект подписан.

```csharp
public byte[] CertRawData { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaProjectPropertyCertRawDataDemo
    {
        public static void Run()
        {
            // Создайте новую книгу с проектом VBA
            Workbook workbook = new Workbook();
            // Не нужно создавать новый VbaProject, так как Workbook уже имеет один

            // Доступ к проекту VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Проверьте, подписан ли VBA проект
            if (vbaProject.IsSigned)
            {
                // Отобразить необработанные данные сертификата, если подписан
                byte[] certData = vbaProject.CertRawData;
                Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));

                // Пример: Сохранить данные сертификата в файл, если они существуют
                if (certData != null && certData.Length > 0)
                {
                    File.WriteAllBytes("VbaCertificate.cer", certData);
                    Console.WriteLine("Certificate saved to file.");
                }
            }
            else
            {
                Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
            }

            // Пример сценария: Загрузить рабочую книгу с подписанным VBA проектом
            string signedWorkbookPath = "SignedWithVba.xlsm";
            if (File.Exists(signedWorkbookPath))
            {
                Workbook signedWorkbook = new Workbook(signedWorkbookPath);
                VbaProject signedVbaProject = signedWorkbook.VbaProject;

                if (signedVbaProject.IsSigned)
                {
                    byte[] signedCertData = signedVbaProject.CertRawData;
                    Console.WriteLine("Loaded workbook's VBA certificate data length: " + 
                        (signedCertData != null ? signedCertData.Length : 0));
                }
            }

            // Сохраните книгу
            workbook.Save("VbaProjectCertRawDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


