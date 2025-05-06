---
title: ContentTypePropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ContentTypePropertyCollection property. Gets the content type property by the specific index
type: docs
url: /net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Gets the content type property by the specific index.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The content type property

### Examples

```csharp
// Called: workbook.ContentTypeProperties[index].IsNillable = true;
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            int index = workbook.ContentTypeProperties.Add(&quot;MK31&quot;, &quot;Simple Data&quot;);
            workbook.ContentTypeProperties[index].IsNillable = true;
            //index= workbook.ContentTypeProperties.Add(&quot;MK32&quot;, &quot;2019-10-17T16:00:00+00:00&quot;, &quot;DateTime&quot;);
            index = workbook.ContentTypeProperties.Add(&quot;MK32&quot;,
                DateTime.Now.ToString(&quot;yyyy-MM-dd&apos;T&apos;hh:mm:ss&quot;), &quot;DateTime&quot;);
            workbook.ContentTypeProperties[index].IsNillable = true;
            workbook.Save(Constants.destPath + &quot;CellsNet46903.xlsx&quot;);
        }
```

### See Also

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Gets the content type property by the property name.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The property name. |

### Return Value

The content type property

### Examples

```csharp
// Called: ContentTypeProperty property = workbook.ContentTypeProperties[&amp;quot;Admin&amp;quot;];
public static void Property_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Add a new content type property
            workbook.ContentTypeProperties.Add(&quot;Admin&quot;, &quot;Aspose&quot;, &quot;text&quot;);

            // Access the newly added property
            ContentTypeProperty property = workbook.ContentTypeProperties[&quot;Admin&quot;];
            
            // Setting properties
            property.Name = &quot;Admin&quot;;
            property.Value = &quot;Aspose&quot;;
            property.Type = &quot;text&quot;;
            property.IsNillable = true;

            // Save the Excel file
            workbook.Save(&quot;ContentTypePropertyExample.xlsx&quot;);
            workbook.Save(&quot;ContentTypePropertyExample.pdf&quot;);
            return;
        }
```

### See Also

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


