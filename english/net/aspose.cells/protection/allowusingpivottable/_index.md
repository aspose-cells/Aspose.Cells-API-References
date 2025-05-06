---
title: Protection.AllowUsingPivotTable
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to manipulate pivot tables on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Represents if the user is allowed to manipulate pivot tables on a protected worksheet.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Examples

```csharp
// Called: protection.AllowUsingPivotTable = true;
public static void Property_AllowUsingPivotTable()
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
            protection.Password = &quot;password123&quot;;
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // Checking if the worksheet is protected with a password
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // Saving the workbook
            workbook.Save(&quot;ProtectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


