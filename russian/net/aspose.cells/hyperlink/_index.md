---
title: "Класс Hyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Hyperlink. Инкапсулирует объект, представляющий гиперссылку"
type: docs
url: /ru/net/aspose.cells/hyperlink/
---
## Hyperlink class

Инкапсулирует объект, представляющий гиперссылку.

```csharp
public class Hyperlink
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Представляет адрес гиперссылки. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Получает диапазон гиперссылки. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Получает тип ссылки. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Возвращает или задает текст ScreenTip для указанной гиперссылки. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Представляет текст, отображаемый для указанной гиперссылки. Значение по умолчанию — адрес гиперссылки. |

## Методы

| Имя | Описание |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Удаляет эту гиперссылку |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Добавление нового листа в объект Workbook
            workbook.Worksheets.Add();
            
            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавление гиперссылки на URL в ячейку "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Получение гиперссылки по индексу
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Установка отображаемого текста этой гиперссылки
            hyperlink.TextToDisplay = "Aspose";
            
            // Установка текста ScreenTip для гиперссылки
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Сохранение файла Excel
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


