---
title: Name.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates whether the name is visible
type: docs
url: /net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Indicates whether the name is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: name.IsVisible = true;
public static void Property_IsVisible()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the worksheet collection
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Access the name collection
            NameCollection names = worksheets.Names;
            
            // Add a new name to the collection
            int nameIndex = names.Add(&quot;MyNamedRange&quot;);
            Name name = names[nameIndex];
            
            // Set the refers to property for the name
            name.RefersTo = &quot;=Sheet1!$A$1:$A$10&quot;;
            
            // Access and modify properties of the name
            name.Comment = &quot;This is a named range for demonstration.&quot;;
            name.IsVisible = true;
            
            // Add another name
            int anotherNameIndex = names.Add(&quot;AnotherNamedRange&quot;);
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = &quot;=Sheet1!$B$1:$B$10&quot;;
            
            // Remove a name by text
            names.Remove(&quot;AnotherNamedRange&quot;);
            
            // Remove a name by index
            names.RemoveAt(nameIndex);
            
            // Clear all names
            names.Clear();
            
            // Save the workbook
            workbook.Save(&quot;NameCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


