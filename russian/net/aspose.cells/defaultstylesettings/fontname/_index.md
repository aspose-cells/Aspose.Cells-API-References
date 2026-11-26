---
title: "DefaultStyleSettings.FontName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DefaultStyleSettings. Получает/задает имя шрифта по умолчанию для книги"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Получает/Устанавливает имя шрифта по умолчанию для книги

```csharp
public string FontName { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки и задать имя шрифта
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Создать новую книгу с параметрами загрузки
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Получить доступ к стилю по умолчанию и проверить имя шрифта
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Создать worksheet и задать значение ячейки
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Сохраните книгу
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### См. также

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


