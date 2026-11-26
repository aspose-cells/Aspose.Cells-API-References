---
title: "LoadOptions.LoadFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Получает формат загрузки"
type: docs
url: /ru/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Получает формат загрузки.

```csharp
public LoadFormat LoadFormat { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Создаёт примерный CSV‑файл
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Создайте LoadOptions для формата CSV и отобразите свойство
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Загрузите CSV с правильными параметрами
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Создайте LoadOptions для формата XLSX и отобразите свойство
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Создайте/сохраните пример файла XLSX
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Загрузите XLSX с правильными параметрами
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Очистите временные файлы
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


