---
title: "ListObject.DataSourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject property. Ruft den Datentyp der Datenquelle der Tabelle ab"
type: docs
url: /de/net/aspose.cells.tables/listobject/datasourcetype/
---
## ListObject.DataSourceType property

Liest den Datentyp der Datenquelle der Tabelle.

```csharp
public TableDataSourceType DataSourceType { get; }
```

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // ListObject erstellen und aus der Sammlung abrufen
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            listObject.DisplayName = "EmployeeTable";

            // DataSourceType abrufen und anzeigen
            TableDataSourceType dataSourceType = listObject.DataSourceType;
            Console.WriteLine("ListObject DataSourceType: " + dataSourceType);

            workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


