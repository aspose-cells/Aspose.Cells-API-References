---
title: "PageSetup.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Копирует настройки разметки страницы"
type: docs
url: /ru/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Копирует настройки разметки страницы.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | PageSetup | Источник. |
| copyOptions | CopyOptions | Параметры копирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Установите свойства PageSetup для первого листа
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // Скопируйте PageSetup с первого листа на второй лист с помощью CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### См. также

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


