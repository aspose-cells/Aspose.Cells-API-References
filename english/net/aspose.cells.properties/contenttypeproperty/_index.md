---
title: Class ContentTypeProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Properties.ContentTypeProperty class. Represents identifier information
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Represents identifier information.

```csharp
public class ContentTypeProperty
```

## Properties

| Name | Description |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Indicates whether the value could be empty. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Returns or sets the name of the object. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Gets and sets the type of the property. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Returns or sets the value of the content type property. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Add a new property.
 workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
//Save the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Add a new property.
 workbook.ContentTypeProperties.Add("Admin", "Aspose", "text")
'Save the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


