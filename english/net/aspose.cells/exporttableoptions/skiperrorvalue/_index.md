---
title: ExportTableOptions.SkipErrorValue
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Indicates whether skip invalid value for the column. For exampleif the column type is decimal the value is greater than decimal.MaxValue and this property is truewe will not throw exception again. The default value is false
type: docs
url: /net/aspose.cells/exporttableoptions/skiperrorvalue/
---
## ExportTableOptions.SkipErrorValue property

Indicates whether skip invalid value for the column. For example,if the column type is decimal ,the value is greater than decimal.MaxValue and this property is true,we will not throw exception again. The default value is false.

```csharp
public bool SkipErrorValue { get; set; }
```

### Examples

```csharp
// Called: eto.SkipErrorValue = true;
[Test]
        public void Property_SkipErrorValue()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;

            Worksheet ws = wb.Worksheets[0];

            ws.Cells["A1"].Value = "Double";
            ws.Cells["A2"].Value = 1.56;

            ExportTableOptions eto = new ExportTableOptions();
            eto.ExportColumnName = true;
            eto.SkipErrorValue = true;
            eto.CheckMixedValueType = true;

            System.Data.DataTable data = ws.Cells.ExportDataTable(0, 0, 2, 1, eto);

           Assert.IsFalse(data.Rows[0][0] is string); //will display "False"
           Assert.AreEqual(1.56,(double)data.Rows[0][0]);

            ws.Cells["A2"].Value = "dummy"; //will force fallback to datatype string
            ws.Cells["A3"].Value = 1.56;

            data = ws.Cells.ExportDataTable(0, 0, 3, 1, eto);

            Assert.IsTrue(data.Rows[1][0] is string); //will display "True"
            Assert.AreEqual("1,56", (string)data.Rows[1][0]); //will display "1.56"

            data = ws.Cells.ExportDataTableAsString(0, 0, 3, 1, true);

           Assert.IsTrue(data.Rows[1][0] is string); //will display "True"
            Assert.AreEqual("1,56", (string)data.Rows[1][0]); //will display "1.56"
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


