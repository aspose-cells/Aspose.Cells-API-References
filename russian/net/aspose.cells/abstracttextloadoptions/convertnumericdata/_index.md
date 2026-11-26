---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractTextLoadOptions. Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Создайте пример CSV‑данных с числовыми и строковыми значениями
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Создайте TxtLoadOptions с параметром ConvertNumericData, установленным в true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Загрузите данные CSV в книгу
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрируйте числовое преобразование
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Продемонстрируйте строковые значения, которые не удалось преобразовать
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Покажите, как кавычные числа всё равно преобразуются, когда ConvertNumericData установлен в true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### См. также

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


