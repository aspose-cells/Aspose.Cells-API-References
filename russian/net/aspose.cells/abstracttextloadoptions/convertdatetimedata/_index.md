---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractTextLoadOptions. Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. Значение по умолчанию — true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Создайте CSV‑данные со строкой даты
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Создайте параметры загрузки текста с ConvertDateTimeData, установленным в false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Загрузите CSV‑данные
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Выведите значения (должны оставаться строками)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Теперь загрузите, установив ConvertDateTimeData в true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Выведите преобразованные значения
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### См. также

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


