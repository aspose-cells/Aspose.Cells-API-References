---
title: Workbook.Colors
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Returns colors in the palette for the spreadsheet
type: docs
url: /net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Returns colors in the palette for the spreadsheet.

```csharp
public Color[] Colors { get; }
```

### Remarks

The palette has 56 entries, each represented by an RGB value.

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.Colors, result.Colors, info + ".Colors");
public static void Property_Colors(Workbook expected, Workbook result, string info)
        {
            AssertHelper.AreEqual(expected.Colors, result.Colors, info + ".Colors");
            StylesTest.Property_Colors(expected.DefaultStyle, result.DefaultStyle, info + ".DefaultStyle");
            Assert.AreEqual(expected.HasMacro, result.HasMacro);
            Assert.AreEqual(expected.AbsolutePath, result.AbsolutePath);
            AssertHelper.equals(expected.Colors, result.Colors, info + ".Colors");
            WorksheetsTest.Property_Colors(expected.Worksheets, result.Worksheets, info + ".Worksheets");
            DataSorterTest.equals(expected.DataSorter, result.DataSorter, info + ".DataSorter");
            Property_Colors(expected.Settings, result.Settings, info);

            Property_Colors(expected.CustomDocumentProperties, result.CustomDocumentProperties, info + ".CustomDocumentProperties");
           // Property_Colors(expected.BuiltInDocumentProperties, result.BuiltInDocumentProperties, info + ".BuiltInDocumentProperties");
            Property_Colors(expected.DataConnections, result.DataConnections, info);
            Property_Colors(expected.ContentTypeProperties, result.ContentTypeProperties, info + ".ContentTypeProperties");
            AssertHelper.AreEqual(expected.RibbonXml, result.RibbonXml, info + ".RibbonXml");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


