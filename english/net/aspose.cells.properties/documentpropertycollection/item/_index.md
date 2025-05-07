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
// Called: Assert.AreEqual(workbook.CustomDocumentProperties["SettingsXML2"].Value.ToString().IndexOf("x000d"), -1);
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "LineBreakTest_GoodSettings.xlsx");
            Assert.AreEqual(workbook.CustomDocumentProperties["SettingsXML2"].Value.ToString().IndexOf("x000d"), -1);
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
// Called: DocumentProperty property1 = cp1[i];
private static void Property_Int32_(
            CustomDocumentPropertyCollection cp1,
            CustomDocumentPropertyCollection cp2)
        {
            Assert.AreEqual(cp1.Count, cp2.Count, "Workbook--CustomDocumentPropertyCollection--Count");
            for (int i = 0; i < cp1.Count; i++)
            {
                DocumentProperty property1 = cp1[i];
                DocumentProperty property2 = cp2[i];
                Assert.AreEqual(property1.Value, property2.Value, "Workbook--DocumentProperty.getValue()");
                Assert.AreEqual(property1.Source, property2.Source, "Workbook--DocumentProperty.getSource()");
                Assert.AreEqual(property1.Type, property2.Type, "Workbook--DocumentProperty.getType()");
            }
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


