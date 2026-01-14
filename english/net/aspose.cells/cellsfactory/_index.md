---
title: Class CellsFactory
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellsFactory class. Utility for instantiating classes of the Cells model
type: docs
url: /net/aspose.cells/cellsfactory/
---
## CellsFactory class

Utility for instantiating classes of the Cells model.

```csharp
public class CellsFactory
```

## Constructors

| Name | Description |
| --- | --- |
| [CellsFactory](cellsfactory/)() | The default constructor. |

## Methods

| Name | Description |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Creates a new style. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Create a new instance of CellsFactory
            CellsFactory factory = new CellsFactory();

            // Use the factory to create a new Style
            Style style = factory.CreateStyle();

            // Customize the style
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Create a new workbook and worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Apply the style to a specific cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Save the workbook to a file
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


