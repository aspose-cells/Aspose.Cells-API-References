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
// Called: workbook.CustomDocumentProperties.Add(&amp;quot;test&amp;quot;, &amp;quot;testvalue&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Password = &quot;1234&quot;;
            workbook.CustomDocumentProperties.Add(&quot;test&quot;, &quot;testvalue&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet47704.xls&quot;);
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
// Called: customProperties.Add(&amp;quot;Revision&amp;quot;, 3);
public static void Method_Int32_()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();

            // Retrieve a list of all custom document properties of the Excel file
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Add custom document properties
            customProperties.Add(&quot;Author&quot;, &quot;John Doe&quot;);
            customProperties.Add(&quot;Revision&quot;, 3);
            customProperties.Add(&quot;LastModified&quot;, DateTime.Now);
            customProperties.Add(&quot;IsFinal&quot;, true);
            customProperties.Add(&quot;Rating&quot;, 4.5);

            // Add a linked custom document property
            customProperties.AddLinkToContent(&quot;LinkedProperty&quot;, &quot;Sheet1!A1&quot;);

            // Update linked property values
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accessing custom document properties
            DocumentProperty authorProperty = customProperties[&quot;Author&quot;];
            DocumentProperty revisionProperty = customProperties[&quot;Revision&quot;];
            DocumentProperty lastModifiedProperty = customProperties[&quot;LastModified&quot;];
            DocumentProperty isFinalProperty = customProperties[&quot;IsFinal&quot;];
            DocumentProperty ratingProperty = customProperties[&quot;Rating&quot;];
            DocumentProperty linkedProperty = customProperties[&quot;LinkedProperty&quot;];

            // Print custom document properties
            Console.WriteLine($&quot;Author: {authorProperty.Value}&quot;);
            Console.WriteLine($&quot;Revision: {revisionProperty.ToInt()}&quot;);
            Console.WriteLine($&quot;Last Modified: {lastModifiedProperty.ToDateTime()}&quot;);
            Console.WriteLine($&quot;Is Final: {isFinalProperty.ToBool()}&quot;);
            Console.WriteLine($&quot;Rating: {ratingProperty.ToDouble()}&quot;);
            Console.WriteLine($&quot;Linked Property: {linkedProperty.Value}&quot;);

            // Save the workbook
            workbook.Save(&quot;CustomDocumentPropertiesExample.xlsx&quot;);
            workbook.Save(&quot;CustomDocumentPropertiesExample.pdf&quot;);
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
            const string propertyName = &quot;CustomDate&quot;;
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
// Called: customProperties.Add(&amp;quot;IsReviewed&amp;quot;, true); // Boolean
public static void Method_Boolean_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set some built-in properties
            builtInProperties.Author = &quot;John Doe&quot;;
            builtInProperties.Title = &quot;Sample Workbook&quot;;
            builtInProperties.Subject = &quot;Demonstration of PropertyType&quot;;
            builtInProperties.Company = &quot;Aspose&quot;;

            // Access the custom document properties
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Add custom properties of different types
            customProperties.Add(&quot;IsReviewed&quot;, true); // Boolean
            customProperties.Add(&quot;ReviewDate&quot;, DateTime.Now); // DateTime
            customProperties.Add(&quot;Rating&quot;, 4.5); // Double
            customProperties.Add(&quot;Pages&quot;, 100); // Number
            customProperties.Add(&quot;Summary&quot;, &quot;This is a sample workbook for demonstrating PropertyType.&quot;); // String

            // Retrieve and display custom properties
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($&quot;Name: {property.Name}, Value: {property.Value}, Type: {property.Type}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;PropertyTypeExample.xlsx&quot;);
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
// Called: wb.CustomDocumentProperties.Add(KeyAverageAge, AverageAgeValue);
[Test]
        public void Method_Double_()
        {
            Workbook wb = new Workbook(FileFormatType.Excel97To2003);

            string KeyAverageAge = &quot;Average Age&quot;;
            double AverageAgeValue = 31.5;

            string KeyDistance = &quot;Distance&quot;;
            float DistanceValue = 2194.5f;

            string AuthorValue = &quot;John Smith&quot;;
            wb.BuiltInDocumentProperties.Author = AuthorValue;
            wb.CustomDocumentProperties.Add(KeyAverageAge, AverageAgeValue);
            wb.CustomDocumentProperties.Add(KeyDistance, DistanceValue);
            wb = Util.ReSave(wb, new XlsSaveOptions(), new LoadOptions(LoadFormat.Excel97To2003));
            Assert.AreEqual(AuthorValue, wb.BuiltInDocumentProperties.Author, &quot;BuiltIn-Author&quot;);
            Assert.AreEqual(AverageAgeValue, wb.CustomDocumentProperties[KeyAverageAge].Value, &quot;Custom-&quot; + KeyAverageAge);
            Assert.AreEqual(DistanceValue, wb.CustomDocumentProperties[KeyDistance].Value, &quot;Custom-&quot; + KeyDistance);
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


