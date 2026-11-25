---
title: "ListObject.DataSourceType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene il tipo di origine dati della tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

Ottiene il tipo di origine dati della tabella.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataSourceTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Crea un oggetto elenco e ottienilo dalla collezione
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            listObject.DisplayName = "EmployeeTable";

            // Ottieni e visualizza DataSourceType
            TableDataSourceType dataSourceType = listObject.DataSourceType;
            Console.WriteLine("ListObject DataSourceType: " + dataSourceType);

            workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


