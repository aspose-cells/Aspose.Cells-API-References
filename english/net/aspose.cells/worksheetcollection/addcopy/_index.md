---
title: WorksheetCollection.AddCopy
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
type: docs
url: /net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Exceptions

| exception | condition |
| --- | --- |
| [CellsException](../../cellsexception/) | Specifies an invalid worksheet name. |

### Examples

```csharp
// Called: int iDesign = wb.Worksheets.AddCopy("Designer");
         //http://www.aspose.com/community/forums/thread/347146.aspx
         public void WorksheetCollection_Method_AddCopy()
         {
             Console.WriteLine("testCELLSNET_40157 ()");
             string infn = path + @"example.xlsx";
             string outfn = destpath + @"template.out.xlsx";

             string infn1 = path + @"example.xls";
             string outfn1 = destpath + @"template.out1.xlsx";


             Workbook wb = new Workbook(infn);
             int iDesign = wb.Worksheets.AddCopy("Designer");
             Worksheet wsDesigner = wb.Worksheets[iDesign];
             wsDesigner.Name = "Copy";
             wb.Save(outfn);
#if WTEST
             Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
             wb = new Workbook(infn1);
             wb.Save(outfn1);
#if WTEST
             Process.Start("explorer.exe", string.Format("\"{0}\"", outfn1));
#endif
         }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Examples

```csharp
// Called: wb.Worksheets.AddCopy(0);
public void WorksheetCollection_Method_AddCopy()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook a = new Workbook();
    a.Copy(wb);
    Assert.IsTrue(a.Worksheets[0].Cells["B6"].EmbeddedImage != null);
    a.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.Worksheets.AddCopy(0);
    Assert.IsTrue(wb.Worksheets[1].Cells["B6"].EmbeddedImage != null);
    wb.Save(Constants.destPath + "example.html");
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copy a group of worksheets.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | The source worksheets. |
| destSheetNames | String[] | The names of the copied sheets. |

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add some sample worksheets
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Populate some data in the worksheets
            workbook.Worksheets["Sheet1"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Prepare source worksheets array
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet1"],
                workbook.Worksheets["Sheet2"]
            };

            // Prepare destination sheet names array
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet1",
                "CopyOfSheet2"
            };

            try
            {
                // Call the AddCopy method with (Worksheet[], String[]) parameters
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Verify the copies were created
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


