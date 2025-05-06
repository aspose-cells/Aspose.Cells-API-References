---
title: CellsHelper.CreateSafeSheetName
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with   then return the rebuilt string value
type: docs
url: /net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |

### Examples

```csharp
// Called: string name = CellsHelper.CreateSafeSheetName(&amp;quot;sheet*/test*/?#&amp;quot;);
[Test]
        public static void Method_String_()
        {
            string name = CellsHelper.CreateSafeSheetName(&quot;sheet*/test*/?#&quot;);
            Assert.AreEqual(&quot;sheet  test   #&quot;, name);
            name = CellsHelper.CreateSafeSheetName(&quot;sheet*/test*/?#&quot;, &apos;A&apos;);
            Assert.AreEqual(&quot;sheetAAtestAAA#&quot;, name);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | String | sheet name to be used |
| replaceChar | Char | character which will be used to replace invalid characters in given sheet name |

### Examples

```csharp
// Called: name = CellsHelper.CreateSafeSheetName(&amp;quot;sheet*/test*/?#&amp;quot;, &amp;apos;A&amp;apos;);
[Test]
        public static void Method_Char_()
        {
            string name = CellsHelper.CreateSafeSheetName(&quot;sheet*/test*/?#&quot;);
            Assert.AreEqual(&quot;sheet  test   #&quot;, name);
            name = CellsHelper.CreateSafeSheetName(&quot;sheet*/test*/?#&quot;, &apos;A&apos;);
            Assert.AreEqual(&quot;sheetAAtestAAA#&quot;, name);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


