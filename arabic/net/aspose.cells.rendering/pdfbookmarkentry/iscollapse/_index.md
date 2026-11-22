---
title: "PdfBookmarkEntry.IsCollapse"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfBookmarkEntry. عندما تكون هذه الخاصية صحيحة سيتقلص إدخال العلامة المرجعية وإلا سيتوسع"
type: docs
url: /ar/net/aspose.cells.rendering/pdfbookmarkentry/iscollapse/
---
## PdfBookmarkEntry.IsCollapse property

عند تكون هذه الخاصية true، سيُطوى bookmarkentry، وإلا سيتوسع.

```csharp
public bool IsCollapse { get; set; }
```

### أمثلة

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

            // إنشاء إدخال علامة مرجعية جذرية
            PdfBookmarkEntry rootEntry = new PdfBookmarkEntry();
            rootEntry.Text = "Annual Report";

            // إنشاء قسم مالي مطوي
            PdfBookmarkEntry financialSection = new PdfBookmarkEntry();
            financialSection.Text = "Financial Data";
            Console.WriteLine("Financial section IsCollapse initial value: " + financialSection.IsCollapse); // Default: False
            
            financialSection.IsCollapse = true; // Collapse this section by default
            Console.WriteLine("Financial section IsCollapse after modification: " + financialSection.IsCollapse); // Now: True

            // إضافة أقسام فرعية ربع سنوية إلى القسم المالي
            financialSection.SubEntry = new System.Collections.ArrayList();
            for (int i = 1; i <= 4; i++)
            {
                PdfBookmarkEntry quarter = new PdfBookmarkEntry();
                quarter.Text = $"Q{i} 2023";
                financialSection.SubEntry.Add(quarter);
            }

            // إنشاء قسم تشغيلي موسع
            PdfBookmarkEntry opsSection = new PdfBookmarkEntry();
            opsSection.Text = "Operations";
            opsSection.IsCollapse = false; // Explicitly expanded

            // بناء تسلسل هرمي للعلامات المرجعية
            rootEntry.SubEntry = new System.Collections.ArrayList();
            rootEntry.SubEntry.Add(financialSection);
            rootEntry.SubEntry.Add(opsSection);

            // تعيين العلامات المرجعية إلى خيارات الحفظ
            saveOptions.Bookmark = rootEntry;

            // حفظ مع العلامات المرجعية المُكوَّنة
            workbook.Save("CollapsibleBookmarks.pdf", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


