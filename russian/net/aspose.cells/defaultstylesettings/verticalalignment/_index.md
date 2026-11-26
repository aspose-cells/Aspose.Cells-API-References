---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DefaultStyleSettings. Получает/устанавливает значение по умолчанию для вертикального выравнивания"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Получает/Устанавливает значение по умолчанию для вертикального выравнивания

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить вертикальное выравнивание по умолчанию в значение Bottom
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите некоторые примерные данные
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Проверьте, что вертикальное выравнивание применено ко всем ячейкам
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Сохраните книгу
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


