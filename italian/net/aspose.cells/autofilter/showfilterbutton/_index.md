---
title: "AutoFilter.ShowFilterButton"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFilter. Indica se il pulsante AutoFilter per questa colonna è visibile"
type: docs
url: /it/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

Indica se il pulsante AutoFilter per questa colonna è visibile.

```csharp
public bool ShowFilterButton { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto elenco/tabella
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // Abilita l'autofiltro e mostra i pulsanti filtro
            table.AutoFilter.ShowFilterButton = true;

            // Salva la cartella di lavoro
            workbook.Save("output_with_filter_buttons.xlsx");

            // Nascondi i pulsanti filtro
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


