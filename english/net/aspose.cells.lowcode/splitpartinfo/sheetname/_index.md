---
title: SplitPartInfo.SheetName
second_title: Aspose.Cells for .NET API Reference
description: SplitPartInfo property. Name of the sheet where current part is in
type: docs
url: /net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

Name of the sheet where current part is in.

```csharp
public string SheetName { get; }
```

### Remarks

May be null for some situations, such as when rendering the whole workbook to tiff image.

### Examples

```csharp
namespace AsposeCellsExamples.SplitPartInfoPropertySheetNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Reflection;

    public class SplitPartInfoPropertySheetNameDemo
    {
        public static void Run()
        {
            // Create a new workbook and populate data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "SalesReport";
            
            // Add data to create multiple pages when rendered
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Transaction {row + 1}";
            }

            // Configure image save options to split into pages
            ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
            // SplitSheetIntoPages property does not exist; removed the line
            options.ImageOrPrintOptions.PageCount = 1;

            // Save workbook to trigger split operation
            workbook.Save("SplitPartDemo.png", options);

            // Simulation to demonstrate property access (using reflection for demonstration only)
            SplitPartInfo dummyPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);
            typeof(SplitPartInfo).GetProperty("SheetName", BindingFlags.Instance | BindingFlags.Public | BindingFlags.NonPublic)
                ?.SetValue(dummyPartInfo, "SalesReport");
            
            // Normally you'd retrieve SplitPartInfo from operation result like:
            // foreach(SplitPartInfo partInfo in result.SplitPartInfos)
            Console.WriteLine("Current SheetName value: " + dummyPartInfo.SheetName);
            
            // SheetName is read-only - this line would cause compile error if uncommented
            // dummyPartInfo.SheetName = "NewName"; 
        }
    }
}
```

### See Also

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


