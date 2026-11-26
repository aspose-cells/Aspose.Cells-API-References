---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Указывает, сохраняется ли как файл flat opc, который может быть сгенерирован Open XML SDK"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Указывает, сохраняется ли как плоский OPC‑файл, который может быть сгенерирован Open XML SDK.

```csharp
public bool AsFlatOpc { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные, чтобы пример имел смысл
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // Создайте экземпляр OoxmlSaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Отобразите значение свойства AsFlatOpc по умолчанию
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Установите AsFlatOpc в true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Сохраните книгу с включённым AsFlatOpc
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // Создайте другие параметры сохранения с отключённым AsFlatOpc
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // Сохраните книгу с отключённым AsFlatOpc
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
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

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


