---
title: OleObject.IsLink
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Returns true if the OleObject links to the file
type: docs
url: /net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Returns true if the OleObject links to the file.

```csharp
public bool IsLink { get; set; }
```

### Examples

```csharp
// Called: if (!ole.IsLink)
[Test]
        public void Property_IsLink()
        {
            Workbook workbook = new Workbook(Constants.sourcePath  + "CELLSNET43894.xlsm");

            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    if (!ole.IsLink)
                    {
                        continue;
                    }

                    Console.WriteLine("OLD ObjectSourceFullName: " + ole.ObjectSourceFullName);
                    string newName = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newName;
                    Console.WriteLine("NEW ObjectSourceFullName: " + ole.ObjectSourceFullName);
                }
            }//foreach

            workbook.Save(Constants.destPath + "CELLSNET43894.xlsm");
            workbook = new Workbook(Constants.destPath + "CELLSNET43894.xlsm");
            Assert.AreEqual(workbook.Worksheets[0].OleObjects[0].ObjectSourceFullName, @"D:\_Work\annual business plan review.docx");

        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


