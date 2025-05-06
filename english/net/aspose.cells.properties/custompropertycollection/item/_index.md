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
// Called: AssertHelper.AreEqual(expected[i].Value, result[i].Value, info + &amp;quot;.StringValue&amp;quot;);
public static void Property_Int32_(CustomPropertyCollection expected, CustomPropertyCollection result, string info)
        {
            if (AssertHelper.checkNull(expected, result, info))
            {
                return;
            }
            int countSrc = expected.Count;
            int countDest = result.Count;
            AssertHelper.AreEqual(countSrc, countDest, info);
            for (int i = 0; i &lt; countSrc &amp;&amp; i &lt; countDest; i++)
            {
                AssertHelper.AreEqual(expected[i].Name, result[i].Name, info + &quot;.Name&quot;);
                AssertHelper.AreEqual(expected[i].Value, result[i].Value, info + &quot;.StringValue&quot;);
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
// Called: Console.WriteLine(book.Worksheets[0].CustomProperties[&amp;quot;tttt&amp;quot;].Value);
[Test]
        public void Property_String_()
        {
            Console.WriteLine(&quot;Property_String_()&quot;);
            //string outfn1 = path + &quot;TEST_SheetCustPrpts.xlsx&quot;;
            //string outfn2 = path + &quot;TEST_SheetCustPrpts_out.xlsx&quot;;
            Workbook book = new Workbook();
            book.Worksheets[0].CustomProperties.Add(&quot;tttt&quot;, &quot;sheet cust property ttt vvv&quot;);
            book = Util.ReSave(book, SaveFormat.Xlsx);
            Console.WriteLine(book.Worksheets[0].CustomProperties[&quot;tttt&quot;].Value);
            //book.Save(outfn2);
        }
```

### See Also

* class [CustomProperty](../../customproperty/)
* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


