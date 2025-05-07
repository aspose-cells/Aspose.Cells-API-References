---
title: SaveOptions.ClearData
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Make the workbook empty after saving the file
type: docs
url: /net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Make the workbook empty after saving the file.

```csharp
public bool ClearData { get; set; }
```

### Examples

```csharp
// Called: txtSaveOptions.ClearData = true;
[Test, Ignore("Not ready to test this yet")]
        public void Property_ClearData()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestWorkbook\\Book1.xls");
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.ClearData = true;
            workbook.Save(Constants.destPath + "testSave.CSV", txtSaveOptions);

            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);           
            workbook = new Workbook(Constants.destPath + "testSave.CSV", loadOptions);
            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Assert.AreEqual("", cells[i, j].StringValue);
                }
            }
            Assert.AreEqual("", cells[0, 1].StringValue);
            Assert.AreEqual("", cells[2, 2].StringValue);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


