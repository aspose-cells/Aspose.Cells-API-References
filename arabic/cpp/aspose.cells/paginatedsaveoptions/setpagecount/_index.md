---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /ar/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
---
## PaginatedSaveOptions::SetPageCount method


Gets or sets the number of pages to save.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetPageCount(int32_t value)
```

## Remarks


Default is System.Int32.MaxValue which means all pages will be rendered.. 

## Examples


```cpp
Aspose::Cells::Startup();
//المثال التالي يوضح كيفية تحويل مجموعة صفحات (3 و 4) في ملف Microsoft Excel إلى PDF.
 //فتح ملف Excel
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//طباعة الصفحة 3 فقط والصفحة 4 في ملف PDF الناتج
//فهرس الصفحة الابتدائي (فهرس يبدأ من 0)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//عدد الصفحات التي سيتم طباعتها
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//حفظ ملف PDF
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
