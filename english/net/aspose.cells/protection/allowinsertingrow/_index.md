---
title: Protection.AllowInsertingRow
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the insertion of rows is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Represents if the insertion of rows is allowed on a protected worksheet

```csharp
public bool AllowInsertingRow { get; set; }
```

### Examples

```csharp
// Called: protection.AllowInsertingRow = true;
public static void Protection_Property_AllowInsertingRow()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accessing the protection settings of the worksheet
            Protection protection = worksheet.Protection;

            // Setting various protection properties
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Checking if the worksheet is protected with a password
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Saving the workbook
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


