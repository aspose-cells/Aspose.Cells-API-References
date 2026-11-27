---
title: "Workbook.DataModel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar datamodellen i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbook/datamodel/
---
## Workbook.DataModel property

Hämtar datamodellen i arbetsboken.

```csharp
public DataModel DataModel { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataModelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till exempeldata i kalkylblad för att skapa en datamodell
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("DepartmentID");
            sheet1.Cells["B1"].PutValue("DepartmentName");
            sheet1.Cells["A2"].PutValue(1);
            sheet1.Cells["B2"].PutValue("HR");
            sheet1.Cells["A3"].PutValue(2);
            sheet1.Cells["B3"].PutValue("IT");

            Worksheet sheet2 = workbook.Worksheets.Add("Employees");
            sheet2.Cells["A1"].PutValue("EmployeeID");
            sheet2.Cells["B1"].PutValue("EmployeeName");
            sheet2.Cells["C1"].PutValue("DepartmentID");
            sheet2.Cells["A2"].PutValue(101);
            sheet2.Cells["B2"].PutValue("John");
            sheet2.Cells["C2"].PutValue(1);
            sheet2.Cells["A3"].PutValue(102);
            sheet2.Cells["B3"].PutValue("Alice");
            sheet2.Cells["C3"].PutValue(2);

            // Demonstrera användning av DataModel-egenskapen
            Console.WriteLine("Data Model Relationships:");
            foreach (DataModelRelationship rel in workbook.DataModel.Relationships)
            {
                Console.WriteLine($"Relationship: {rel.PrimaryKeyTable}.{rel.PrimaryKeyColumn} -> {rel.ForeignKeyTable}.{rel.ForeignKeyColumn}");
            }

            Console.WriteLine("\nData Model Tables:");
            foreach (DataModelTable table in workbook.DataModel.Tables)
            {
                Console.WriteLine($"Table: {table.Name}");
            }

            // Spara arbetsboken
            workbook.Save("WorkbookWithDataModel.xlsx");
        }
    }
}
```

### Se även

* class [DataModel](../../../aspose.cells.datamodels/datamodel/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


