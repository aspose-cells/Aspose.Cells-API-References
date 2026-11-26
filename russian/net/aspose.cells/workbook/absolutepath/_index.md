---
title: "Workbook.AbsolutePath"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает и задает абсолютный путь к файлу"
type: docs
url: /ru/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Получает и задает абсолютный путь к файлу.

```csharp
public string AbsolutePath { get; set; }
```

### Примечания

Используется только для внешних ссылок.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook sourceBook = new Workbook();
            
            // Добавить несколько листов
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Сохраните workbook, чтобы получить физический путь
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Повторно откройте workbook, чтобы продемонстрировать AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Используйте свойство AbsolutePath для построения полного пути
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Добавьте гиперссылки, используя путь
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Сохранить изменённую книгу
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


