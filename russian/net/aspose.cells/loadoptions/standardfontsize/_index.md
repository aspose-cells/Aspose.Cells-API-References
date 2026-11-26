---
title: "LoadOptions.StandardFontSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Устанавливает размер шрифта по умолчанию"
type: docs
url: /ru/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Устанавливает размер шрифта по умолчанию.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки HTML и установите StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Получите доступ к первому листу и ячейкам
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Установите некоторый пример текста и проверьте свойства шрифта
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


