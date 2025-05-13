---
title: CustomProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected[i].Name, result[i].Name, info + ".Name");
public static void CustomProperty_Property_Name(CustomPropertyCollection expected, CustomPropertyCollection result, string info)
        {
            if (AssertHelper.checkNull(expected, result, info))
            {
                return;
            }
            int countSrc = expected.Count;
            int countDest = result.Count;
            AssertHelper.AreEqual(countSrc, countDest, info);
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                AssertHelper.AreEqual(expected[i].Name, result[i].Name, info + ".Name");
                AssertHelper.AreEqual(expected[i].Value, result[i].Value, info + ".StringValue");
            }
        }
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


