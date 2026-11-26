---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли обрезать завершающие пустые ячейки в строке. По умолчанию false"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Указывает, следует ли удалять завершающие пустые ячейки в строке. По умолчанию false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Примечания

При сохранении в режиме LightCells и если [`ExportArea`](../exportarea/) не указана, эта опция не действует, и строка будет расширена только до последней ячейки, предоставленной реализацией [`LightCellsDataProvider`](../lightcellsdataprovider/)

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавьте примерные данные
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Сохранить без обрезки завершающих пустых ячеек (по умолчанию)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Сохранить с обрезкой завершающих пустых ячеек
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


