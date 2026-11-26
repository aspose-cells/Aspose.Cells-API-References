---
title: "PdfSaveOptions.Producer"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает и задает производителя сгенерированного pdf‑документа"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Получает и задаёт производителя сгенерированного PDF‑документа.

```csharp
public string Producer { get; set; }
```

### Примечания

Если значение равно null или действительная LICENSE не установлена, будет использована строка Aspose.Cells vVERSION.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // Создайте параметры сохранения PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Установите свойство Producer
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Сохранить в поток памяти
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Проверьте, что свойство Producer установлено
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
                }
            }
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


