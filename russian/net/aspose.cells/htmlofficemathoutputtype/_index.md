---
title: "Перечисление HtmlOfficeMathOutputType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.HtmlOfficeMathOutputType. Представляет способ экспорта OfficeMath в HTML"
type: docs
url: /ru/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Представляет способ экспорта OfficeMath в HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Image | `0` | Преобразует OfficeMath в HTML как изображение, указанное тегом &lt;img&gt;. |
| MathML | `1` | Преобразует OfficeMath в HTML с использованием MathML. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить OfficeMath в ячейку A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установить тип вывода OfficeMath в Image
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Сохранить с типом вывода Image
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Изменить тип вывода на MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Сохранить с типом вывода MathML
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


