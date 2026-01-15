---
title: Cells.OdsCellFields
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the list of fields of ods
type: docs
url: /net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Gets the list of fields of ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the Cells collection
            Cells cells = worksheet.Cells;

            try
            {
                // Access the OdsCellFields property (read-only)
                var odsCellFields = cells.OdsCellFields;

                // Display information about the OdsCellFields collection
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Iterate through the OdsCellFields collection
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Demonstrate updating field values
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


