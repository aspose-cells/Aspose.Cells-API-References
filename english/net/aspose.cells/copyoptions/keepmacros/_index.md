---
title: CopyOptions.KeepMacros
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether keeping macros
type: docs
url: /net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Indicates whether keeping macros;

```csharp
public bool KeepMacros { get; set; }
```

### Remarks

Only for copying workbook.

### Examples

```csharp
// Called: KeepMacros = true,
public static void Property_KeepMacros()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Create a new workbook to copy data into
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Create a CopyOptions object
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Copy the data from the source worksheet to the destination worksheet
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Save the destination workbook
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


