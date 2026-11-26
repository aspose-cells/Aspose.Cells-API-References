---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей может уменьшить размер файла без влияния на визуальное отображение. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в книге для генерируемого HTML, например в сценарии, когда позже требуется восстановить книгу из сгенерированного HTML, пожалуйста, установите это свойство в значение false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Указывает, исключать ли неиспользуемые стили. Для генерируемых HTML‑файлов исключение неиспользуемых стилей уменьшает размер файла без влияния на визуальное отображение. Поэтому значение по умолчанию этого свойства — true. Если пользователю необходимо сохранить все стили в рабочей книге для генерируемого HTML (например, чтобы позже восстановить книгу из HTML), установите значение свойства в false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные с разными стилями
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Настройте параметры сохранения HTML для исключения неиспользуемых стилей
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Сохранить рабочую книгу с параметрами HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


