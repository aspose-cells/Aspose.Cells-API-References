---
title: OleObject.DisplayAsIcon
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. True if the specified object is displayed as an icon and the image will not be auto changed
type: docs
url: /net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True if the specified object is displayed as an icon and the image will not be auto changed.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Examples

```csharp
// Called: oleObjTest.DisplayAsIcon = (true);
private static void Property_DisplayAsIcon(Worksheet sheetTest, string pdf)
        {
            byte[] imgTest = File.ReadAllBytes(Constants.sourcePath + &quot;image1.png&quot;);
            byte[] dataTest = File.ReadAllBytes(pdf);
            int oleObjIndexTest = sheetTest.OleObjects.Add(0, 0, 50, 50, imgTest);
            OleObject oleObjTest = sheetTest.OleObjects[oleObjIndexTest];

            //Set embedded ole object data.
            oleObjTest.DisplayAsIcon = (true);
            oleObjTest.ObjectSourceFullName = pdf;
            oleObjTest.ObjectData = (dataTest);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


