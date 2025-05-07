---
title: Shape.FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoFillFormat object that contains fill formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: MsoFillFormat fill = shape.FillFormat;
[Test]
        public void Property_FillFormat()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsJava40157.xls");

            for (int i = 0, size = wb.Worksheets.Count; i < size; i++)
            {
                Worksheet sheet = wb.Worksheets[i];
                foreach (Object o in sheet.Shapes)
                {
                    Shape shape = (Shape)o;

                    MsoFillFormat fill = shape.FillFormat;

                }
            }

            wb.Save(Constants.destPath + "CellsJava40157.xls");

        }
```

### See Also

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


