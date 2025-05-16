---
title: NameCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove an array of name
type: docs
url: /net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Remove an array of name

```csharp
public void Remove(string[] names)
```

| Parameter | Type | Description |
| --- | --- | --- |
| names | String[] | The names' text. |

### Examples

```csharp
namespace AsposeCellsExamples.NameCollectionMethodRemoveWithStringArrayDemo
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Get the NameCollection from the workbook
            NameCollection names = workbook.Worksheets.Names;
            
            // Add some named ranges to demonstrate removal
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Prepare the array of names to remove
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Call the Remove method with String[] parameter
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Display remaining names
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Remove the name.

```csharp
public void Remove(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The name text. |

### Examples

```csharp
// Called: workbook.Worksheets.Names.Remove("Source!EHC_Admin");
public void NameCollection_Method_Remove()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    int count = workbook.Worksheets.Names.Count;
    //workbook.Worksheets.DeleteName("Source!EHC_Admin");
    workbook.Worksheets.Names.Remove("Source!EHC_Admin");
    Worksheet sheet = workbook.Worksheets["Test"];
    Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");

    range.Name = "EHC_Admin";
    Assert.AreEqual(workbook.Worksheets.Names.Count, count);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


