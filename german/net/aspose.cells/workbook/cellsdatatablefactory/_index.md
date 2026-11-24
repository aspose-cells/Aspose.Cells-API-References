---
title: "Workbook.CellsDataTableFactory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook‑Eigenschaft. Gibt die Fabrik zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten zurück."
type: docs
url: /de/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Gibt die Fabrik zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten zurück

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Beispiele

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // CellsDataTableFactory aus der Workbook‑Eigenschaft abrufen.
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Datentabelle aus einer Liste erstellen.
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Daten in Arbeitsblatt importieren
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Ausgaben speichern
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


