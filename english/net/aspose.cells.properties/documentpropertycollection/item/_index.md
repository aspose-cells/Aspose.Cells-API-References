---
title: DocumentPropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: DocumentPropertyCollection property. Returns a DocumentProperty object by the name of the property
type: docs
url: /net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Returns a [`DocumentProperty`](../../documentproperty/) object by the name of the property.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The case-insensitive name of the property to retrieve. |

### Remarks

Returns null if a property with the specified name is not found.

### Examples

```csharp
// Called: Assert.AreEqual(doc.CustomDocumentProperties[&amp;quot;text1&amp;quot;].Value.ToString(), &amp;quot;text2&amp;quot;);
[Test]
        public void Property_String_()
        {
            WorkbookMetadata doc = new WorkbookMetadata(Constants.sourcePath + &quot;CellsNet44144.xls&quot;, new MetadataOptions(MetadataType.DocumentProperties));
            doc.CustomDocumentProperties.Add(&quot;text1&quot;, &quot;text2&quot;);
            doc.CustomDocumentProperties.Add(&quot;num1&quot;, 1);
            doc.Save(Constants.destPath + &quot;dest.xls&quot;);
            Workbook workbook = new Workbook(Constants.destPath + &quot;dest.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;Data&quot;);
            Assert.AreEqual(doc.CustomDocumentProperties[&quot;text1&quot;].Value.ToString(), &quot;text2&quot;);

            
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Returns a [`DocumentProperty`](../../documentproperty/) object by index.

```csharp
public DocumentProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | Zero-based index of the [`DocumentProperty`](../../documentproperty/) to retrieve. |

### Examples

```csharp
// Called: DocumentProperty propSrc = expected[i];
public static void Property_Int32_(DocumentPropertyCollection expected, DocumentPropertyCollection resultProperties, string info)
        {
            if (AssertHelper.checkNull(expected, resultProperties, info))
            {
                return;
            }
            int countSrc = expected.Count;
            int countDest = resultProperties.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + &quot;.Count&quot;);
            for (int i = 0; i &lt; countSrc &amp;&amp; i &lt; countDest; i++)
            {
                DocumentProperty propSrc = expected[i];
                DocumentProperty propDest = resultProperties[i];
                Property_Int32_(propSrc, propDest, info + &quot;.DocumentProperty&quot;);
            }
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


