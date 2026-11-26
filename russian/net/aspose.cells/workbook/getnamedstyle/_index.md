---
title: "Workbook.GetNamedStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Возвращает именованный стиль из пула стилей"
type: docs
url: /ru/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Получает именованный стиль из пула стилей.

```csharp
public Style GetNamedStyle(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | имя стиля |

### Возвращаемое значение

именованный стиль, возможно null.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetNamedStyleWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько именованных стилей
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Создать примерные данные
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Получить рабочий лист и ячейки
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Получить именованные стили
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Применить стили к данным
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Сохраните книгу
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


