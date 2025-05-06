---
title: ContentTypePropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ContentTypePropertyCollection method. Adds content type property information
type: docs
url: /net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Adds content type property information.

```csharp
public int Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |

### Examples

```csharp
// Called: ctps.Add(&amp;quot;dddd&amp;quot;, &amp;quot;gggg&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;mm.xlsx&quot;);
            ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
            //ContentTypeProperty ctp = new ContentTypeProperty(ctps);
            //ctp.Name = &quot;dddd&quot;;
            //ctp.Value = &quot;gggg&quot;;
            ctps.Add(&quot;dddd&quot;, &quot;gggg&quot;);
            wb.Save(Constants.savePivottablePath + &quot;wangtao.xlsx&quot;);
            wb = new Workbook(Constants.openPivottablePath + &quot;AfterUpload.xlsx&quot;);
            wb.Save(Constants.savePivottablePath + &quot;40590.xlsx&quot;);
        }
```

### See Also

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Adds content type property information.

```csharp
public int Add(string name, string value, string type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |
| type | String | The type of the content type property. |

### Examples

```csharp
// Called: workbook.ContentTypeProperties.Add(&amp;quot;ss&amp;quot;, &amp;quot;bb&amp;quot;, &amp;quot;text&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add(&quot;ss&quot;, &quot;bb&quot;, &quot;text&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet43276.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet43276.xlsx&quot;);
        }
```

### See Also

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


