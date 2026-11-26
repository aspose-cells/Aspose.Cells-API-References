---
title: "WorkbookSettings.PaperSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Возвращает и задаёт размер бумаги по умолчанию для печати"
type: docs
url: /ru/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Получает и задает размер бумаги по умолчанию для печати.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Примечания

Если настройка размера бумаги отсутствует, MS Excel будет использовать настройки принтера по умолчанию.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите размер бумаги на A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Проверьте, что размер бумаги установлен правильно в первом листе
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


