---
title: LoadOptions.Password
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and set the password of the workbook
type: docs
url: /net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Gets and set the password of the workbook.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: loadOptions.Password = "xixi";
[Test]
        public void Property_Password()
        {
            LoadOptions loadOptions = new LoadOptions();
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET-46163/unEncrypted.ods", loadOptions);
            Assert.AreEqual("test encrypt.", wb.Worksheets[0].Cells["C6"].Value);
            wb.Settings.Password = "xixi";

            wb.Save(Constants.destPath + "CELLSNET-46163_Cs.ods");

            loadOptions.Password = "xixi";
            wb = new Workbook(Constants.destPath + "CELLSNET-46163_Cs.ods", loadOptions);
            Assert.AreEqual("test encrypt.", wb.Worksheets[0].Cells["C6"].Value);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


