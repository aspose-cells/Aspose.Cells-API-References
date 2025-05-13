---
title: NameCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove the name at the specific index
type: docs
url: /net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Remove the name at the specific index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index of the Name to be removed. |

### Remarks

Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred, setting Name.RefersTo as null is better.

### Examples

```csharp
// Called: names.RemoveAt(nameIndex);
public static void NameCollection_Method_RemoveAt()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the worksheet collection
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Access the name collection
            NameCollection names = worksheets.Names;
            
            // Add a new name to the collection
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Set the refers to property for the name
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Access and modify properties of the name
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Add another name
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Remove a name by text
            names.Remove("AnotherNamedRange");
            
            // Remove a name by index
            names.RemoveAt(nameIndex);
            
            // Clear all names
            names.Clear();
            
            // Save the workbook
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


