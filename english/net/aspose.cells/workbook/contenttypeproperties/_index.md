---
title: Workbook.ContentTypeProperties
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the list of ContentTypeProperty objects in the workbook
type: docs
url: /net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Gets the list of [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) objects in the workbook.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Examples

```csharp
// Called: Check(expected.ContentTypeProperties, result.ContentTypeProperties, info + &amp;quot;.ContentTypeProperties&amp;quot;);
public static void Property_ContentTypeProperties(Workbook expected, Workbook result, string info)
        {
            AssertHelper.AreEqual(expected.Colors, result.Colors, info + &quot;.Colors&quot;);
            StylesTest.Property_ContentTypeProperties(expected.DefaultStyle, result.DefaultStyle, info + &quot;.DefaultStyle&quot;);
            Assert.AreEqual(expected.HasMacro, result.HasMacro);
            Assert.AreEqual(expected.AbsolutePath, result.AbsolutePath);
            AssertHelper.equals(expected.Colors, result.Colors, info + &quot;.Colors&quot;);
            WorksheetsTest.Property_ContentTypeProperties(expected.Worksheets, result.Worksheets, info + &quot;.Worksheets&quot;);
            DataSorterTest.equals(expected.DataSorter, result.DataSorter, info + &quot;.DataSorter&quot;);
            Property_ContentTypeProperties(expected.Settings, result.Settings, info);

            Property_ContentTypeProperties(expected.CustomDocumentProperties, result.CustomDocumentProperties, info + &quot;.CustomDocumentProperties&quot;);
           // Property_ContentTypeProperties(expected.BuiltInDocumentProperties, result.BuiltInDocumentProperties, info + &quot;.BuiltInDocumentProperties&quot;);
            Property_ContentTypeProperties(expected.DataConnections, result.DataConnections, info);
            Property_ContentTypeProperties(expected.ContentTypeProperties, result.ContentTypeProperties, info + &quot;.ContentTypeProperties&quot;);
            AssertHelper.AreEqual(expected.RibbonXml, result.RibbonXml, info + &quot;.RibbonXml&quot;);
        }
```

### See Also

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


