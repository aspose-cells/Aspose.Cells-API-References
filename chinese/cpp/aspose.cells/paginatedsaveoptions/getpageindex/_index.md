---
title: Aspose::Cells::PaginatedSaveOptions::GetPageIndex method
linktitle: GetPageIndex
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPageIndex method. Gets or sets the 0-based index of the first page to save in C++.'
type: docs
weight: 2300
url: /zh/cpp/aspose.cells/paginatedsaveoptions/getpageindex/
---
## PaginatedSaveOptions::GetPageIndex method


Gets or sets the 0-based index of the first page to save.

```cpp
int32_t Aspose::Cells::PaginatedSaveOptions::GetPageIndex()
```

## Remarks


Default is 0. 

## Examples


```cpp
Aspose::Cells::Startup();
//以下示例展示了如何将 Microsoft Excel 文件中的页面范围（第 3 页和第 4 页）渲染为 PDF。
 //打开 Excel 文件
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//在输出的 PDF 中仅打印第 3 页和第 4 页
//起始页面索引（基于 0 的索引）
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//要打印的页面数量
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//保存 PDF 文件
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
