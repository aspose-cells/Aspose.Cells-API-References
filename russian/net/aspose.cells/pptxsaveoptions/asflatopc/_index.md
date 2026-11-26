---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PptxSaveOptions. Указывает, сохраняется ли как плоский файл opc, который может быть сгенерирован с помощью Open XML SDK"
type: docs
url: /ru/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

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

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте пример рабочего листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Создать экземпляр PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Отобразить значение по умолчанию для AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Установить свойство в true, чтобы продемонстрировать его использование
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Сохранить книгу в формате PPTX с включённой опцией
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


