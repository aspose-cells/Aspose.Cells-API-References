---
title: Class ReferredArea
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ReferredArea class. Represents a referred area by the formula
type: docs
url: /net/aspose.cells/referredarea/
---
## ReferredArea class

Represents a referred area by the formula.

```csharp
public class ReferredArea
```

## Properties

| Name | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | The end column of the area. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | The end row of the area. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Get the external file name if this is an external reference. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Indicates whether this is an area. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Indicates whether this area contains all rows(entire column). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Indicates whether this area contains all columns(entire row). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Indicates whether this is an external link. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Indicates which sheet this reference is in. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Names of all the worksheets this instance references to. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | The start column of the area. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | The start row of the area. |

## Methods

| Name | Description |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Gets cell value with given offset from the top-left of this area. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Gets cell value with given offset from the top-left of this area. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Gets cell values in this area. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Gets cell values in this area. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaDemo
    {
        public static void ReferredAreaExample()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Define the referred area
            ReferredArea referredArea = new ReferredArea();

            // Displaying the properties of the referred area
            Console.WriteLine("IsExternalLink: " + referredArea.IsExternalLink);
            Console.WriteLine("ExternalFileName: " + referredArea.ExternalFileName);
            Console.WriteLine("SheetName: " + referredArea.SheetName);
            Console.WriteLine("IsEntireRow: " + referredArea.IsEntireRow);
            Console.WriteLine("IsEntireColumn: " + referredArea.IsEntireColumn);
            Console.WriteLine("IsArea: " + referredArea.IsArea);
            Console.WriteLine("StartColumn: " + referredArea.StartColumn);
            Console.WriteLine("EndColumn: " + referredArea.EndColumn);
            Console.WriteLine("StartRow: " + referredArea.StartRow);
            Console.WriteLine("EndRow: " + referredArea.EndRow);

            // Use methods of ReferredArea
            object values = referredArea.GetValues();
            Console.WriteLine("Values: " + values);

            object value = referredArea.GetValue(1, 1);
            Console.WriteLine("Value at offset (1, 1): " + value);

            string referenceAddress = referredArea.ToString();
            Console.WriteLine("Reference Address: " + referenceAddress);

            // Save the workbook
            workbook.Save("ReferredAreaExample.xlsx");

            return;
        }
    }

    public class ReferredArea
    {
        public bool IsExternalLink { get; }
        public string ExternalFileName { get; }
        public string SheetName { get; }
        public bool IsEntireRow { get; }
        public bool IsEntireColumn { get; }
        public bool IsArea { get; }
        public int EndColumn { get; }
        public int StartColumn { get; }
        public int EndRow { get; }
        public int StartRow { get; }

        public object GetValues()
        {
            // Placeholder for getting values
            return null;
        }

        public object GetValues(bool calculateFormulas)
        {
            // Placeholder for getting values with formula calculation
            return null;
        }

        public object GetValue(int rowOffset, int colOffset)
        {
            // Placeholder for getting a value at a specific offset
            return null;
        }

        public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
        {
            // Placeholder for getting a value at a specific offset with formula calculation
            return null;
        }

        public override string ToString()
        {
            // Placeholder for converting the area to a string
            return "Sheet1!A1:C3";
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


