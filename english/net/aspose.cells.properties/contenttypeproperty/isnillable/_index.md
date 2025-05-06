---
title: ContentTypeProperty.IsNillable
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Indicates whether the value could be empty
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indicates whether the value could be empty.

```csharp
public bool IsNillable { get; set; }
```

### Examples

```csharp
// Called: workbook.ContentTypeProperties[index].IsNillable = true;
[Test]
        public void Property_IsNillable()
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

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


