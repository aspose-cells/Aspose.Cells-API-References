---
title: CustomDocumentPropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CustomDocumentPropertyCollection method. Creates a new custom document property of the PropertyType.String data type
type: docs
url: /net/aspose.cells.properties/customdocumentpropertycollection/add/
---
## Add(string, string) {#add_4}

Creates a new custom document property of the **PropertyType.String** data type.

```csharp
public DocumentProperty Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | String | The value of the property. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: doc.CustomDocumentProperties.Add("text1", "text2");
[Test]
        public void Method_String_()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "CellsNet44144.xlsm", new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            doc.Save(Constants.destPath + "dest.xlsm");
            Workbook workbook = new Workbook(Constants.destPath + "dest.xlsm");
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Data");
            Assert.AreEqual(doc.CustomDocumentProperties["text1"].Value.ToString(), "text2");


        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_2}

Creates a new custom document property of the **PropertyType.Number** data type.

```csharp
public DocumentProperty Add(string name, int value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Int32 | The value of the property. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: doc.CustomDocumentProperties.Add("num1", 1);
[Test]
        public void Method_Int32_()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + "CellsNet44144.xlsb", new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            doc.Save(Constants.destPath + "dest.xlsb");
            Workbook workbook = new Workbook(Constants.destPath + "dest.xlsb");
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Data");
            Assert.AreEqual(doc.CustomDocumentProperties["text1"].Value.ToString(), "text2");


        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, DateTime) {#add_3}

Creates a new custom document property of the **PropertyType.DateTime** data type.

```csharp
public DocumentProperty Add(string name, DateTime value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | DateTime | The value of the property. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: workbook.CustomDocumentProperties.Add(propertyName, new DateTime(2010, 8, 30, 16, 26, 17, DateTimeKind.Local));
[Test]
        public void Method_DateTime_()
        {
            const string propertyName = "CustomDate";
            var workbook = new Workbook();//I use a simple template file. 
            workbook.CustomDocumentProperties.Add(propertyName, new DateTime(2010, 8, 30, 16, 26, 17, DateTimeKind.Local));
            var workbookAfter = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            Assert.AreEqual(Convert.ToDateTime(workbook.CustomDocumentProperties[propertyName].Value),
                Convert.ToDateTime(workbookAfter.CustomDocumentProperties[propertyName].Value));
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool) {#add}

Creates a new custom document property of the **PropertyType.Boolean** data type.

```csharp
public DocumentProperty Add(string name, bool value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Boolean | The value of the property. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: customProperties.Add("IsFinal", true);
public static void Method_Boolean_()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();

            // Retrieve a list of all custom document properties of the Excel file
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Add custom document properties
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Add a linked custom document property
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Update linked property values
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accessing custom document properties
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Print custom document properties
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Save the workbook
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, double) {#add_1}

Creates a new custom document property of the **PropertyType.Float** data type.

```csharp
public DocumentProperty Add(string name, double value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| value | Double | The value of the property. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: customProperties.Add("Rating", 4.5); // Double
public static void Method_Double_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set some built-in properties
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Access the custom document properties
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Add custom properties of different types
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Retrieve and display custom properties
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Save the workbook
            workbook.Save("PropertyTypeExample.xlsx");
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


