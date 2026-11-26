---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Указывает, повторяются ли формулы с итоговой строкой"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Указывает, повторяются ли формулы с строкой подытога.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyRepeatFormulasWithSubtotalDemo
    {
        public static void Run()
        {
            // Создать примерный DataTable
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // Добавьте примерные данные
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // Создать новую книгу с формулой шаблона
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Настроить шаблон со смарт‑маркировками и формулой
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // Создать дизайнер и установить RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // Обработать шаблон
            designer.Process();

            // Проверить, что формула была повторена для каждой строки
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

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


