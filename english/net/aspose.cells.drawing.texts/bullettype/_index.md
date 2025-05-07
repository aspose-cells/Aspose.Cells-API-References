---
title: Enum BulletType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.BulletType enum. Represents the type of the bullet
type: docs
url: /net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Represents the type of the bullet.

```csharp
public enum BulletType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No bullet. |
| Character | `1` | Character bullet. |
| Picture | `2` | Image bullet. |
| AutoNumbered | `3` | Automatic numbered bullet. |

### Examples

```csharp
// Called: BulletType bulletType = noneBulletValue.Type;
public static void Type_BulletType()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding text to a cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Create a TextBox to apply bullet settings
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Create an instance of NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Check the type of bullet (should be None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Save the workbook to demonstrate the changes
            workbook.Save("NoneBulletValueExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


