---
title: "PivotTable.DataField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект PivotField, представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только когда в области данных присутствует два или более поля данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Возвращает объект [`PivotField`](../../pivotfield/), представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только когда в области данных присутствует два или более полей данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea() .

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotTable.ValuesField. Этот метод будет удалён через 12 месяцев, начиная с октября 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Получить доступ и изменить свойства DataField
            // Позиция только для чтения, поэтому мы продемонстрируем другие свойства
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Сохраните книгу
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


