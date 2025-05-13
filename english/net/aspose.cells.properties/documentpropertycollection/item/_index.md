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
// Called: wb.Worksheets.CustomDocumentProperties[key].Value = value;
public void DocumentPropertyCollection_Property_Item(Workbook wb)
        {
            string key = "TemplateGUID";
            object value = "the value";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            else
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
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
public static void DocumentPropertyCollection_Property_Item(DocumentPropertyCollection expected, DocumentPropertyCollection resultProperties, string info)
        {
            if (AssertHelper.checkNull(expected, resultProperties, info))
            {
                return;
            }
            int countSrc = expected.Count;
            int countDest = resultProperties.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                DocumentProperty propSrc = expected[i];
                DocumentProperty propDest = resultProperties[i];
                DocumentPropertyCollection_Property_Item(propSrc, propDest, info + ".DocumentProperty");
            }
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


