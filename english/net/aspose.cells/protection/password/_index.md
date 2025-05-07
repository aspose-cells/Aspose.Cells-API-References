---
title: Protection.Password
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents the password to protect the worksheet
type: docs
url: /net/aspose.cells/protection/password/
---
## Protection.Password property

Represents the password to protect the worksheet.

```csharp
public string Password { get; set; }
```

### Remarks

If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.

### Examples

```csharp
// Called: protection.Password = "password123";
public static void Property_Password()
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


