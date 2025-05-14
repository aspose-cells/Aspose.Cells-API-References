---
title: DocumentProperty.Value
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Gets or sets the value of the property
type: docs
url: /net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Gets or sets the value of the property.

```csharp
public object Value { get; set; }
```

### Examples

```csharp
// Called: hyperlinkBase.Value = "http://www.svd.se"; // This has no effect
public static void DocumentProperty_Property_Value()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Workbook workbook = new Workbook(USBankConstants.sourcePath + "Blank.xlsx");
            designer.Workbook = workbook;

            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.svd.se"; // This has no effect

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "SomeTitle"; // This sets the Title.

            string output = USBankConstants.resultPath + "Hyperlink_result.xlsx";
            workbook.Save(output);
           
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


