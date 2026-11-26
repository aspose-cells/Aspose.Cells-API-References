---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, отображается ли подпись заголовка строки в отчете сводной таблицы. Указывает, отображать ли подписи полей и выпадающие списки фильтров"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Указывает, отображается ли подпись заголовка строки в отчете сводной таблицы. Указывает, отображать ли подписи полей и выпадающие списки фильтров

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotTable.ShowHeaders. Этот метод будет удалён через 12 месяцев, начиная с апреля 2026 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Добавить примерные данные для сводной таблицы
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Продемонстрировать свойство ShowRowHeaderCaption
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // Сохраните книгу
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


