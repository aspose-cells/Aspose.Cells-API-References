---
title: "Перечисление XAdESType."
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DigitalSignatures.XAdESType. Тип XML Advanced Electronic Signature (XAdES)."
type: docs
url: /ru/net/aspose.cells.digitalsignatures/xadestype/
---
## XAdESType enumeration

Тип XML Advanced Electronic Signature (XAdES).

```csharp
public enum XAdESType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | XAdES отключён. |
| XAdES | `1` | Базовый XAdES. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.IO;
    using System.Security.Cryptography.X509Certificates;

    public class XAdESTypeDemo
    {
        public static void XAdESTypeExample()
        {
            // Исходный каталог.
            string sourceDir = "path_to_source_directory";
            // Каталог вывода.
            string outputDir = "path_to_output_directory";
            // Загрузить книгу.
            Workbook workbook = new Workbook(Path.Combine(sourceDir, "XAdESTypeExample_original.xlsx"));

            // Установить пароль для файла PFX.
            string password = "pfxPassword";
            // Путь к файлу PFX.
            string pfxPath = Path.Combine(sourceDir, "pfxFile.pfx");

            // Создать цифровую подпись.
            DigitalSignature signature = new DigitalSignature(File.ReadAllBytes(pfxPath), password, "testXAdES", DateTime.Now);
            // Установить тип XAdES.
            signature.XAdESType = XAdESType.XAdES;

            // Создать коллекцию цифровых подписей.
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Установить цифровую подпись в книгу.
            workbook.SetDigitalSignature(dsCollection);

            // Сохранить книгу с цифровой подписью.
            workbook.Save(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));

            // Проверить цифровую подпись
            Workbook signedWorkbook = new Workbook(Path.Combine(outputDir, "XAdESSignatureSupport_out.xlsx"));
            DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();

            foreach (DigitalSignature ds in signatures)
            {
                Console.WriteLine($"Comments: {ds.Comments}");
                Console.WriteLine($"Sign Time: {ds.SignTime}");
                Console.WriteLine($"Is Valid: {ds.IsValid}");
                Console.WriteLine($"XAdES Type: {ds.XAdESType}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


