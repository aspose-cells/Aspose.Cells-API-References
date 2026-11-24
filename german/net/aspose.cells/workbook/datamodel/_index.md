---
title: "Workbook.DataModel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt das Datenmodell in der Arbeitsmappe zurück"
type: docs
url: /de/net/aspose.cells/workbook/datamodel/
---
## Workbook.DataModel property

Liest das Datenmodell im Arbeitsbuch.

```csharp
public DataModel DataModel { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Beispieldaten zu Arbeitsblättern hinzufügen, um ein Datenmodell zu erstellen
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

            // Demonstrieren Sie die Verwendung der DataModel‑Eigenschaft
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

            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookWithDataModel.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataModel](../../../aspose.cells.datamodels/datamodel/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


