---
title: "WorkbookDesigner.UpdateReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Указывает, будут ли ссылки в других листах обновлены"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Указывает, будут ли обновляться ссылки в других листах.

```csharp
public bool UpdateReference { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Создать пример набора данных
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Создайте дизайнер рабочей книги
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Установите свойство UpdateReference в true
            designer.UpdateReference = true;
            
            // Создайте новую рабочую книгу с шаблоном
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте умные маркеры
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Обработать дизайнер
            designer.Process();
            
            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


