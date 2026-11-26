---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Получает и задает стиль заголовка"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Получает и задает стиль заголовка.

```csharp
public Style TitleStyle { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyTitleStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример JSON-данных
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Создать пользовательский стиль для заголовков
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // Настроить параметры импорта JSON
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // Импортировать данные JSON с пользовательским стилем заголовка
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Автоматически подгонять столбцы для лучшей видимости
            worksheet.AutoFitColumns();

            // Сохраните книгу
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


