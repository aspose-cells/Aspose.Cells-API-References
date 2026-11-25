---
title: "Workbook.CellsDataTableFactory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene la fabbrica per creare ICellsDataTable da oggetti personalizzati"
type: docs
url: /it/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Ottiene la factory per costruire ICellsDataTable da oggetti personalizzati

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Ottieni CellsDataTableFactory dalla proprietà workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Crea una tabella dati da un elenco
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importa dati nel foglio di lavoro
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Salva i risultati
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


