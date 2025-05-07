---
title: Validation.Formula2
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Represents the value or expression associated with the data validation
type: docs
url: /net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Represents the value or expression associated with the data validation.

```csharp
public string Formula2 { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=ABS(#REF!)", vldt.Formula2, "Copied formula2 of validation");
[Test]
        public void Property_Formula2()
        {
            Workbook wbDest = new Workbook(FileFormatType.Excel97To2003);
            Workbook wbSrc = new Workbook(FileFormatType.Xlsx);
            Worksheet sheet = wbSrc.Worksheets[0];
            sheet.Name = "Copied";
            sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[0];
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=ABS($A$1048000)", "=ABS($B$1048000)");
            Validation vldt = sheet.Validations[sheet.Validations.Add(CellArea.CreateCellArea(0, 0, 0, 3))];
            vldt.Operator = OperatorType.Between;
            vldt.Formula1 = "=ABS($A$1048000)";
            vldt.Formula2 = "=ABS($B$1048000)";
            wbDest.Combine(wbSrc);
            sheet = wbDest.Worksheets["Copied"];
            fcc = sheet.ConditionalFormattings[0];
            Assert.AreEqual("=ABS(#REF!)", fcc[0].Formula1, "Copied formula1 of format condition");
            Assert.AreEqual("=ABS(#REF!)", fcc[0].Formula2, "Copied formula2 of format condition");
            vldt = sheet.Validations[0];
            Assert.AreEqual("=ABS(#REF!)", vldt.Formula1, "Copied formula1 of validation");
            Assert.AreEqual("=ABS(#REF!)", vldt.Formula2, "Copied formula2 of validation");
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


