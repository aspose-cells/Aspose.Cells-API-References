---
title: "FilterColumn.IsDropdownVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FilterColumn. Indica se il pulsante AutoFilter per questa colonna è visibile"
type: docs
url: /it/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Indica se il pulsante AutoFilter per questa colonna è visibile.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // Applica AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Ottieni la colonna del filtro
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Mostra il menu a discesa inizialmente
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Nascondi il menu a discesa
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Salva la cartella di lavoro
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


