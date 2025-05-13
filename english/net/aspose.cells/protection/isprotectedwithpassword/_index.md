---
title: Protection.IsProtectedWithPassword
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Indicates whether the worksheets is protected with password
type: docs
url: /net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Indicates whether the worksheets is protected with password.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Examples

```csharp
// Called: bool isProtectedWithPassword = protection.IsProtectedWithPassword;
public static void Protection_Property_IsProtectedWithPassword()
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


