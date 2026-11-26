---
title: "HtmlSaveOptions.ExportSimilarBorderStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать HTML или MHT файл в Excel, оставьте значение по умолчанию. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Указывает, экспортировать ли похожий стиль границы, когда стиль границы не поддерживается браузерами. Если вы хотите импортировать файл html или mht в Excel, пожалуйста, оставьте значение по умолчанию. Значение по умолчанию — false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пример данных с границами
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["B1"].PutValue("Similar Border");
            worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["C1"].PutValue("Different Border");
            worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));

            // Создать параметры сохранения HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportSimilarBorderStyle = true // Demonstrate the property
            };

            // Сохраните книгу
            workbook.Save("output.html", htmlSaveOptions);
        }

        private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = borderType;
            style.Borders[BorderType.BottomBorder].LineStyle = borderType;
            style.Borders[BorderType.LeftBorder].LineStyle = borderType;
            style.Borders[BorderType.RightBorder].LineStyle = borderType;
            return style;
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


