---
title: "PivotField.IsRepeatItemLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, следует ли повторять метки поля в строковой или столбцовой области. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Указывает, следует ли повторять метки поля в области строк или столбцов. Значение по умолчанию — false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");

            // Получить доступ к листу, содержащему сводную таблицу
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Получить доступ к сводной таблице
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Включите повторение меток элементов для первого строкового поля
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Включите повторение меток элементов для первого столбцового поля
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


