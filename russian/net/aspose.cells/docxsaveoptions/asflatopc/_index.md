---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Указывает, сохраняется ли как плоский opc‑файл, который может быть сгенерирован с помощью Open XML SDK"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

Указывает, сохраняется ли как плоский opc‑файл, который может быть сгенерирован Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // Инициализируйте DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Отобразите значение свойства AsFlatOpc по умолчанию
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Установите AsFlatOpc в true, чтобы продемонстрировать его использование
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Сохраните книгу в формате DOCX с настроенными параметрами
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


