---
title: Name.R1C1RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets or sets a R1C1 reference of the Name
type: docs
url: /net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Gets or sets a R1C1 reference of the [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new name to the names collection
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Set R1C1 reference for the name
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Verify the reference was set correctly
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Save the workbook
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


