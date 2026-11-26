---
title: "TxtSaveOptions.TxtSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор TxtSaveOptions. Создает параметры сохранения текстового файла"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Создает параметры сохранения текстового файла.

```csharp
public TxtSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Продемонстрировать конструктор TxtSaveOptions
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "|";
            
            // Сохраните с пользовательским разделителем
            workbook.Save("output.txt", txtSaveOptions);
            
            Console.WriteLine("File saved with custom separator successfully.");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Создает параметры сохранения текстового файла.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveFormat | SaveFormat | Формат файла. Он должен быть Csv или Tsv, иначе сохранённый формат будет автоматически установлен как Csv. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Вызовите метод #ctor с параметром SaveFormat
                TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
                
                // Настройте параметры сохранения
                saveOptions.Separator = ',';
                saveOptions.Encoding = Encoding.UTF8;
                saveOptions.QuoteType = TxtValueQuoteType.Always;
                
                Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
                
                // Сохраните книгу с настроенными параметрами
                workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


