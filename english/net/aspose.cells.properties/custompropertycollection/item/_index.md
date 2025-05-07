---
title: CustomPropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CustomPropertyCollection property. Gets the custom property by the specific index
type: docs
url: /net/aspose.cells.properties/custompropertycollection/item/
---
## CustomPropertyCollection indexer (1 of 2)

Gets the custom property by the specific index.

```csharp
public CustomProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The custom property

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected[i].Name, result[i].Name, info + ".Name");
public static void Property_Int32_(CustomPropertyCollection expected, CustomPropertyCollection result, string info)
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

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## CustomPropertyCollection indexer (2 of 2)

Gets the custom property by the property name.

```csharp
public CustomProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The property name. |

### Return Value

The custom property

### Examples

```csharp
// Called: Console.WriteLine(book.Worksheets[0].CustomProperties["tttt"].Value);
[Test]
        public void Property_String_()
        {
            Console.WriteLine("Property_String_()");
            //string outfn1 = path + "TEST_SheetCustPrpts.xlsx";
            //string outfn2 = path + "TEST_SheetCustPrpts_out.xlsx";
            Workbook book = new Workbook();
            book.Worksheets[0].CustomProperties.Add("tttt", "sheet cust property ttt vvv");
            book = Util.ReSave(book, SaveFormat.Xlsx);
            Console.WriteLine(book.Worksheets[0].CustomProperties["tttt"].Value);
            //book.Save(outfn2);
        }
```

### See Also

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


