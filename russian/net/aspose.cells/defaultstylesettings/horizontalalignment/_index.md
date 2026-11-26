---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DefaultStyleSettings. Получает/устанавливает значение по умолчанию для горизонтального выравнивания"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Получает/Устанавливает значение по умолчанию для горизонтального выравнивания

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Установите горизонтальное выравнивание, чтобы продемонстрировать свойство
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


