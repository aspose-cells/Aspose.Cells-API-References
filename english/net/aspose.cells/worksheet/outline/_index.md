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
// Called: OutlineTest.equals(expected.Outline, result.Outline, info + ".Outline");
public static void Worksheet_Property_Outline(Worksheet expected, Worksheet result, string info)
        {
            if (AssertHelper.checkNull(expected, result, info))
            {
                return;
            }
            info = info + "["+ expected.Name+"]";

            CheckOptions(expected,result,info);
            AutoFilterTest.equals(expected.AutoFilter, result.AutoFilter, info + ".AutoFilter");
        


            ConditionalFormattingsTest.equals(expected.ConditionalFormattings, result.ConditionalFormattings, info + ".ConditionalFormattings");
            Worksheet_Property_Outline(expected.CustomProperties, result.CustomProperties, info + ".CustomProperties");
            HPageBreaksTest.equals(expected.HorizontalPageBreaks, result.HorizontalPageBreaks, info + ".HPageBreaks");
            HyperlinksTest.equals(expected.Hyperlinks, result.Hyperlinks, info + ".Hyperlinks");
            OutlineTest.equals(expected.Outline, result.Outline, info + ".Outline");
            PageSetupTest.equals(expected.PageSetup, result.PageSetup, info + ".PageSetup");
            PivotTablesTest.equals(expected.PivotTables, result.PivotTables, info + ".PivotTables");
            ProtectionTest.equals(expected.Protection, result.Protection, info + ".Protection");
            ValidationsTest.equals(expected.Validations, result.Validations, info + ".Validations");
            VPageBreaksTest.equals(expected.VerticalPageBreaks, result.VerticalPageBreaks, info + ".VPageBreaks");
            CellsTest.equals(expected, result, info + ".Cells");
            ShapesTest.Worksheet_Property_Outline(expected.Shapes, result.Shapes, info + ".Shape");



        }
```

### See Also

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


