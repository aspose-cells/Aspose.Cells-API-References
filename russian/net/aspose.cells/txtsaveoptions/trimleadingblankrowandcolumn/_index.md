---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли удалять начальные пустые строки и столбцы, как это делает MS Excel. По умолчанию true"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Указывает, следует ли удалять ведущие пустые строки и столбцы, как делает MS Excel. По умолчанию true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Примечания

То же правило, что и в MS Excel: строка/столбец не считается пустым, если у него есть пользовательский стиль, даже если в нём нет данных ячеек. При сохранении в режиме LightCells эта опция не оказывает влияния. Пользователь должен управлять диапазоном вывода с помощью реализации [`LightCellsDataProvider`](../lightcellsdataprovider/) или указав [`ExportArea`](../exportarea/).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Создайте пример рабочей книги с некоторыми данными и пустыми строками/столбцами
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте данные с начальными пустыми строками и столбцами
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Сохранить без удаления начальных пустых элементов
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Сохранить с удалением начальных пустых элементов
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


