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
            Workbook w = new Workbook(Constants.sourcePath + @&quot;xlsx\CELLSJAVA-43875.xlsx&quot;);
            w.Save(Constants.destPath + &quot;CELLSJAVA43875.xlsb&quot;);
            w = new Workbook(Constants.destPath + &quot;CELLSJAVA43875.xlsb&quot;);
            w.Save(Constants.destPath + &quot;CELLSJAVA43875.xlsx&quot;);
            w = new Workbook(Constants.destPath + &quot;CELLSJAVA43875.xlsx&quot;);
            Assert.AreEqual(32767, w.Settings.DefaultImageResolution);
            Assert.IsFalse(w.Settings.DiscardImageEditData);
          

        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


