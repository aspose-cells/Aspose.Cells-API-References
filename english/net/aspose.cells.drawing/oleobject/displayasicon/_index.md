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
// Called: Console.WriteLine("is ole display as icon: " + ole.DisplayAsIcon);
[Test]
        public void Property_DisplayAsIcon()
        {
            Console.WriteLine("Property_DisplayAsIcon()");
            string infn = path + "Test_OleDisPlayAsIconAttr.xlsx";
            string outfn = Constants.destPath + "Test_OleDisPlayAsIconAttr_out.xlsx";

            Workbook workbook = new Workbook(infn);
            OleObject ole = workbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("is ole display as icon: " + ole.DisplayAsIcon);
            workbook.Save(outfn);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


