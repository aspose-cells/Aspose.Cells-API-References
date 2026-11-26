---
title: "Workbook.GetDigitalSignature"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Получает цифровую подпись из файла"
type: docs
url: /ru/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Получает цифровую подпись из файла.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Вызовите метод GetDigitalSignature для получения цифровых подписей
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Отобразить информацию о цифровых подписях
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // Сохраните книгу
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


