---
title: FormatCondition.Type
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets whether the conditional format Type
type: docs
url: /net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Gets and sets whether the conditional format Type.

```csharp
public FormatConditionType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(FormatConditionType.Expression, fc.Type, &amp;quot;Type&amp;quot;);
public static void Property_Type(FormatCondition fc, int fcsIndex, int n)
        {
            if (fcsIndex == 0 &amp;&amp; n == 1)
            {
                Assert.AreEqual(FormatConditionType.CellValue, fc.Type, &quot;Type&quot;);
                Assert.AreEqual(OperatorType.Between, fc.Operator);
                Assert.AreEqual(&quot;=IU65536&quot;, fc.Formula1, &quot;Formula1&quot;);
                string fml = fc.Formula2;
                if (!string.IsNullOrEmpty(fml) &amp;&amp; fml[0] != &apos;=&apos;)
                {
                    fml = &quot;=&quot; + fml;
                }
                Assert.AreEqual(&quot;=100&quot;, fml, &quot;Formula2&quot;);
                AssertHelper.equals(Color.Red, fc.Style.BackgroundColor, &quot;&quot;);
            }
            else if (fcsIndex == 0 &amp;&amp; n == 2)
            {
                Assert.AreEqual(FormatConditionType.CellValue, fc.Type, &quot;Type&quot;);
                Assert.AreEqual(OperatorType.Between, fc.Operator);
                string fml = fc.Formula1;
                if (!string.IsNullOrEmpty(fml) &amp;&amp; fml[0] != &apos;=&apos;)
                {
                    fml = &quot;=&quot; + fml;
                }
                Assert.AreEqual(&quot;=50&quot;, fml, &quot;Formula1&quot;);
                fml = fc.Formula2;
                if (!string.IsNullOrEmpty(fml) &amp;&amp; fml[0] != &apos;=&apos;)
                {
                    fml = &quot;=&quot; + fml;
                }
                Assert.AreEqual(&quot;=100&quot;, fml, &quot;Formula2&quot;);
            }
            else if (fcsIndex == 1 &amp;&amp; n == 1)
            {
                Assert.AreEqual(FormatConditionType.Expression, fc.Type, &quot;Type&quot;);
                string fml = fc.Formula1;
                if (!string.IsNullOrEmpty(fml) &amp;&amp; fml[0] != &apos;=&apos;)
                {
                    fml = &quot;=&quot; + fml;
                }
                Assert.AreEqual(&quot;=10&quot;, fml, &quot;Formula1&quot;);
                AssertHelper.equals(Color.Blue, fc.Style.BackgroundColor, &quot;&quot;);
            }
            else if (fcsIndex == 2 &amp;&amp; n == 1)
            {
                Assert.AreEqual(FormatConditionType.CellValue, fc.Type, &quot;Type&quot;);
                Assert.AreEqual(OperatorType.LessOrEqual, fc.Operator);
                string fml = fc.Formula1;
                if (!string.IsNullOrEmpty(fml) &amp;&amp; fml[0] != &apos;=&apos;)
                {
                    fml = &quot;=&quot; + fml;
                }
                Assert.AreEqual(&quot;=2.18&quot;, fml, &quot;Formula1&quot;);
                AssertHelper.equals(Color.Red, fc.Style.Font.Color, &quot;FormatCondition.Style.ForegroundColor&quot;);
            }
        }
```

### See Also

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


