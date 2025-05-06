---
title: Worksheet.Outline
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the outline on this worksheet
type: docs
url: /net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Gets the outline on this worksheet.

```csharp
public Outline Outline { get; }
```

### Examples

```csharp
// Called: OutlineTest.equals(expected.Outline, result.Outline, info + &amp;quot;.Outline&amp;quot;);
public static void Property_Outline(Worksheet expected, Worksheet result, string info)
        {
            if (AssertHelper.checkNull(expected, result, info))
            {
                return;
            }
            info = info + &quot;[&quot;+ expected.Name+&quot;]&quot;;

            CheckOptions(expected,result,info);
            AutoFilterTest.equals(expected.AutoFilter, result.AutoFilter, info + &quot;.AutoFilter&quot;);
        


            ConditionalFormattingsTest.equals(expected.ConditionalFormattings, result.ConditionalFormattings, info + &quot;.ConditionalFormattings&quot;);
            Property_Outline(expected.CustomProperties, result.CustomProperties, info + &quot;.CustomProperties&quot;);
            HPageBreaksTest.equals(expected.HorizontalPageBreaks, result.HorizontalPageBreaks, info + &quot;.HPageBreaks&quot;);
            HyperlinksTest.equals(expected.Hyperlinks, result.Hyperlinks, info + &quot;.Hyperlinks&quot;);
            OutlineTest.equals(expected.Outline, result.Outline, info + &quot;.Outline&quot;);
            PageSetupTest.equals(expected.PageSetup, result.PageSetup, info + &quot;.PageSetup&quot;);
            PivotTablesTest.equals(expected.PivotTables, result.PivotTables, info + &quot;.PivotTables&quot;);
            ProtectionTest.equals(expected.Protection, result.Protection, info + &quot;.Protection&quot;);
            ValidationsTest.equals(expected.Validations, result.Validations, info + &quot;.Validations&quot;);
            VPageBreaksTest.equals(expected.VerticalPageBreaks, result.VerticalPageBreaks, info + &quot;.VPageBreaks&quot;);
            CellsTest.equals(expected, result, info + &quot;.Cells&quot;);
            ShapesTest.Property_Outline(expected.Shapes, result.Shapes, info + &quot;.Shape&quot;);



        }
```

### See Also

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


