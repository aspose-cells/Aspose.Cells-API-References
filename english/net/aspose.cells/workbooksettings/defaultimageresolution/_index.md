---
title: WorkbookSettings.DefaultImageResolution
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets default resolution of image
type: docs
url: /net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Gets and sets default resolution of image.

```csharp
public int DefaultImageResolution { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(32767, w.Settings.DefaultImageResolution);
[Test]
        public void Property_DefaultImageResolution()
        {
            Workbook w = new Workbook(Constants.sourcePath + @"xlsx\CELLSJAVA-43875.xlsx");
            w.Save(Constants.destPath + "CELLSJAVA43875.xlsb");
            w = new Workbook(Constants.destPath + "CELLSJAVA43875.xlsb");
            w.Save(Constants.destPath + "CELLSJAVA43875.xlsx");
            w = new Workbook(Constants.destPath + "CELLSJAVA43875.xlsx");
            Assert.AreEqual(32767, w.Settings.DefaultImageResolution);
            Assert.IsFalse(w.Settings.DiscardImageEditData);
          

        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


