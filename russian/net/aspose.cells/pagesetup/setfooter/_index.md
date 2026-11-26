---
title: "PageSetup.SetFooter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает скрипт, форматирующий нижний колонтитул Excel‑файла"
type: docs
url: /ru/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Устанавливает скриптовое форматирование нижнего колонтитула Excel‑файла.

```csharp
public void SetFooter(int section, string footerScript)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerScript | String | Скрипт формата нижнего колонтитула. |

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

Например: "&amp;Arial,Bold&amp;8Footer Note"

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


