---
title: "LoadOptions.StandardFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Устанавливает имя шрифта по умолчанию"
type: docs
url: /ru/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Устанавливает имя шрифта по умолчанию

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте DefaultStyleSettings. Это свойство будет удалено через 12 месяцев, начиная с марта 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Создайте пример файла Excel в памяти
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Установите параметры загрузки с StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Загрузите книгу с указанным шрифтом
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Продемонстрируйте, что шрифт установлен, проверяя стиль по умолчанию
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


