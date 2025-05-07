---
title: Worksheet.CustomProperties
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets an object representing the identifier information associated with a worksheet
type: docs
url: /net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Gets an object representing the identifier information associated with a worksheet.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Remarks

Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

### Examples

```csharp
// Called: Check(expected.CustomProperties, result.CustomProperties, info + ".CustomProperties");
public static void Property_CustomProperties(Worksheet expected, Worksheet result, string info)
        {
            if (AssertHelper.checkNull(expected, result, info))
            {
                return;
            }
            info = info + "["+ expected.Name+"]";

            CheckOptions(expected,result,info);
            AutoFilterTest.equals(expected.AutoFilter, result.AutoFilter, info + ".AutoFilter");
        


            ConditionalFormattingsTest.equals(expected.ConditionalFormattings, result.ConditionalFormattings, info + ".ConditionalFormattings");
            Property_CustomProperties(expected.CustomProperties, result.CustomProperties, info + ".CustomProperties");
            HPageBreaksTest.equals(expected.HorizontalPageBreaks, result.HorizontalPageBreaks, info + ".HPageBreaks");
            HyperlinksTest.equals(expected.Hyperlinks, result.Hyperlinks, info + ".Hyperlinks");
            OutlineTest.equals(expected.Outline, result.Outline, info + ".Outline");
            PageSetupTest.equals(expected.PageSetup, result.PageSetup, info + ".PageSetup");
            PivotTablesTest.equals(expected.PivotTables, result.PivotTables, info + ".PivotTables");
            ProtectionTest.equals(expected.Protection, result.Protection, info + ".Protection");
            ValidationsTest.equals(expected.Validations, result.Validations, info + ".Validations");
            VPageBreaksTest.equals(expected.VerticalPageBreaks, result.VerticalPageBreaks, info + ".VPageBreaks");
            CellsTest.equals(expected, result, info + ".Cells");
            ShapesTest.Property_CustomProperties(expected.Shapes, result.Shapes, info + ".Shape");



        }
```

### See Also

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


