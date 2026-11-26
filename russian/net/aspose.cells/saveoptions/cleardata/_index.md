---
title: "SaveOptions.ClearData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Делает книгу пустой после сохранения файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Сделать книгу пустой после сохранения файла.

```csharp
public bool ClearData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить тестовые данные
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // Настроить параметры сохранения с ClearData = false
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Сохраните книгу
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Перезагрузить, чтобы проверить, что данные сохранены
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


