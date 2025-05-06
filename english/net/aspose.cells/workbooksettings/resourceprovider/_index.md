---
title: WorkbookSettings.ResourceProvider
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the stream provider for external resource such as loading image data for picture of type LinkToFile
type: docs
url: /net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.ResourceProvider = new StreamProvider();
[Test]
        public void Property_ResourceProvider()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44353.xlsx&quot;);
            workbook.Settings.ResourceProvider = new StreamProvider();
            workbook.Save(Constants.destPath + &quot;CellsNet44353.pdf&quot;);
        }
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


