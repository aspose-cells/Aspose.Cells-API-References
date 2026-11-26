---
title: "HtmlSaveOptions.ExportArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает экспортируемую CellArea текущего активного листа. Если задать этот атрибут, область печати текущего активного листа будет опущена. При сохранении файла в HTML будет экспортирована только указанная область."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Получает или задаёт область ячеек (CellArea) для экспорта текущего активного листа. Если задать этот атрибут, область печати текущего активного листа будет игнорироваться. При сохранении в HTML будет экспортирована только указанная область.

```csharp
public CellArea ExportArea { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните лист некоторыми данными
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Установите параметры сохранения HTML с областью экспорта
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Сохранить книгу с указанной областью экспорта
            workbook.Save("output.html", options);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


