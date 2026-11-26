---
title: "PageSetup.SetHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт форматирования заголовка Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Устанавливает скриптовое форматирование верхнего колонтитула Excel‑файла.

```csharp
public void SetHeader(int section, string headerScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerScript | String | Скрипт формата заголовка. |

### Примечания

Команды скрипта:

| **Команда** | **Описание** |
| --- | --- |
| &amp;P | Текущий номер страницы |
| &amp;N | Количество страниц |
| &amp;D | Текущая дата |
| &amp;T | Текущее время |
| &amp;A | Имя листа |
| &amp;F | Имя файла без пути |
| &amp;"&lt;FontName&gt;" | Имя шрифта, например: &amp;"Arial" |
| &amp;"&lt;FontName&gt;, &lt;FontStyle&gt;" | Имя шрифта и стиль, например: &amp;"Arial,Bold" |
| &amp;&lt;FontSize&gt; | Размер шрифта. Если эта команда сопровождается простым числом, которое будет напечатано в заголовке, оно будет отделено от высоты шрифта пробелом. |
| &amp;K&lt;RRGGBB&gt; | Цвет шрифта, например (RED): &amp;KFF0000 |
| &amp;G | Скрипт изображения |

Например: "&amp;Arial,Bold&amp;8Header Note"

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите разные секции заголовка с помощью различных команд
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


