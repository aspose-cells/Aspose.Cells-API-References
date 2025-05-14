---
title: NoneBulletValue.Type
second_title: Aspose.Cells for .NET API Reference
description: NoneBulletValue property. Gets the type of the bullets value
type: docs
url: /net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

Gets the type of the bullet's value.

```csharp
public override BulletType Type { get; }
```

### Examples

```csharp
// Called: BulletType bulletType = noneBulletValue.Type;
public static void NoneBulletValue_Property_Type()
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

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


