---
title: PageCount
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает количество страниц для сохранения.
type: docs
weight: 240
url: /ru/net/aspose.cells/pdfsaveoptions/pagecount/
---
## PdfSaveOptions.PageCount property

Получает или задает количество страниц для сохранения.

```csharp
public int PageCount { get; set; }
```

### Примечания

По умолчанию используется System.Int32.MaxValue, что означает, что будут отображаться все страницы..

### Примеры

В следующем примере показано, как преобразовать диапазон страниц (3 и 4) в файле Microsoft Excel в формат PDF.

```csharp
//Открываем файл Excel
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions options = new PdfSaveOptions();

// Печатать только страницу 3 и страницу 4 в выходном PDF
// Индекс начальной страницы (индекс на основе 0)
options.PageIndex = 3;
//Количество страниц для печати
options.PageCount = 2;

// Сохраняем файл PDF
wb.Save("output.pdf", options);
```

### Смотрите также

* class [PdfSaveOptions](../../pdfsaveoptions)
* пространство имен [Aspose.Cells](../../pdfsaveoptions)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
