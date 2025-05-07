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
// Called: Assert.AreEqual("Japanese", docProperty1.Value);
[Test]
        public void Property_Value()
        {
            //lineFormat.Weight = 0.0;
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava42580.xls");
            BuiltInDocumentPropertyCollection bdpc = workbook.Worksheets.BuiltInDocumentProperties;

            DocumentProperty docProperty1 = bdpc["Language"];
            Assert.AreEqual("Japanese", docProperty1.Value);
            workbook.Save(Constants.destPath + "CellsJava42580.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsJava42580.xlsx");
            docProperty1 = bdpc["Language"];
            Assert.AreEqual("Japanese", docProperty1.Value);
            Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


