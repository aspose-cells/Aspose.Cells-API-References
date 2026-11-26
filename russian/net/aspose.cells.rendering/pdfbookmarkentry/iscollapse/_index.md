---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfBookmarkEntry. Когда это свойство истинно, запись закладки будет свернута, иначе будет развёрнута."
type: docs
url: /ru/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

Если это свойство истинно, bookmarkentry будет свернут, иначе он будет развернут.

```csharp
public bool IsCollapse { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyIsCollapseDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Создать корневую запись закладки
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // Создать свернутый финансовый раздел
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // Добавить квартальные подразделы к финансовому разделу
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // Создать развернутый операционный раздел
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // Построить иерархию закладок
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // Назначить закладки параметрам сохранения
            saveOptions.Bookmark = rootEntry;

            // Сохранить с настроенными закладками
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### См. также

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


