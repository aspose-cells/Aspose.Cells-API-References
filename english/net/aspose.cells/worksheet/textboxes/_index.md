---
title: Worksheet.TextBoxes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a TextBox collection
type: docs
url: /net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Gets a [`TextBox`](../../../aspose.cells.drawing/textbox/) collection.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Examples

```csharp
// Called: int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
[Test]
        public void Property_TextBoxes()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47325.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a new textbox to the collection.
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            var sheet = workbook.Worksheets[0];
            var textBox = sheet.TextBoxes[0];
            string str = "<Font Style=\"FONT-FAMILY: Arial; FONT-SIZE: 9pt; COLOR: #000000;TEXT-ALIGN: left;VERTICAL-ALIGN: top;\">< Font Style = \"FONT-FAMILY: Arial;FONT-SIZE: 9pt;COLOR: #000000;TEXT-ALIGN: left;\">";

            textBox.HtmlText = str;
            //  var chart = textBox.Characters(0, 1);//IF we comment it, there is no issue then
           Assert.AreEqual(0xC6,textBox.HtmlText.Length);
            workbook.Save(Constants.destPath + "CellsNet47325.xlsx");

        }
```

### See Also

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


