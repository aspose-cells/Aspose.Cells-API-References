---
title: WorkbookDesigner.UpdateEmptyStringAsNull
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. If TRUE Null will be inserted if the value is 
type: docs
url: /net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

If TRUE, Null will be inserted if the value is "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Examples

```csharp
// Called: designer.UpdateEmptyStringAsNull = true;
[Test]
        public void Property_UpdateEmptyStringAsNull()
        {
            DataSet ds1 = new DataSet();
            ds1.ReadXml(Constants.sourcePath + "SmartMarker/CELLSNET46344.xml");

            Workbook workbook = new Workbook(Constants.sourcePath + "SmartMarker/CELLSNET46344.xlsx");
            object b = ds1.Tables[0].Rows[2][0];
            string thridValue = ds1.Tables[0].Rows[2][0].ToString();
            if (thridValue == string.Empty)
            {
                Console.WriteLine("The third value is empty");
            }
            // Instantiate a new WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.UpdateEmptyStringAsNull = true;
            designer.UpdateReference = true;

            // Specify the Workbook
            designer.Workbook = workbook;

            designer.SetDataSource(ds1.Tables["comparison"]);
            designer.Process();
            workbook.CalculateFormula();
            Assert.IsTrue(workbook.Worksheets[0].Cells["B3"].BoolValue);
            workbook.Save(Constants.destPath + "CELLSNET46344.xlsx");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


