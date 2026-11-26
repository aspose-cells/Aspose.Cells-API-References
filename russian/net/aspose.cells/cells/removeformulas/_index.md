---
title: "Cells.RemoveFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Удаляет все формулы и заменяет их значением формулы"
type: docs
url: /ru/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Удаляет все формулы и заменяет их значением формулы.

```csharp
public void RemoveFormulas()
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // Создать пример набора данных
            DataSet ds = new DataSet();

            // Создать и заполнить таблицу Master
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Создать и заполнить таблицу OppLineItems
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Создать новую книгу
            Workbook wkb = new Workbook();
            
            // Использовать WorkbookDesigner для привязки данных
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Добавить формулу для демонстрации удаления
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Сначала вычислить формулы
            wkb.CalculateFormula();

            // Удалить все формулы из листа
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Сохраните книгу
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


