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

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Set up some data and a formula that references a range
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Create a formula that references the range A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Get the referred areas from the formula
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Get the first referred area
                    ReferredArea referredArea = referredAreas[0];

                    // Display basic properties of the referred area
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Get values from the referred area
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Get a specific value from the referred area
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Display the reference address
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Save the workbook
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


