---
title: "Класс PdfBookmarkEntry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Rendering.PdfBookmarkEntry класс. PdfBookmarkEntry является записью в закладках PDF. Если свойство Text текущего экземпляра равно null, текущий экземпляр будет скрыт, а дочерние элементы будут вставлены на текущем уровне."
type: docs
url: /ru/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry является записью в закладках PDF. Если свойство Text текущего экземпляра равно null или "", текущий экземпляр будет скрыт, а дочерние элементы будут вставлены на текущем уровне.

```csharp
public class PdfBookmarkEntry
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | Ячейка, к которой привязана ссылка закладки. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Получает или задает имя назначения. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Если это свойство истинно, bookmarkentry будет свернут, иначе он будет развернут. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Если это свойство истинно, bookmarkentry будет развернут, иначе он будет свернут. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | Подзапись закладки. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Заголовок закладки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // Создайте новую рабочую книгу и добавьте листы.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Получите ячейки с каждого листа.
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Поместите значения в ячейки.
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Создайте корневой PdfBookmarkEntry.
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Создайте дочерние PdfBookmarkEntries.
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // Добавьте дочерние записи к корневой записи.
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // Создайте PdfSaveOptions и установите закладку.
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Сохраните рабочую книгу как PDF с закладками.
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


