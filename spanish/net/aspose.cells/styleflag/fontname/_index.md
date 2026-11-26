---
title: "StyleFlag.FontName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del nombre de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

Se aplicará la configuración del nombre de fuente.

```csharp
public bool FontName { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de ejemplo
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // Crear estilos con diferentes nombres de fuente
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // Aplicar estilo de encabezado con StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // Aplicar estilo de precio con StyleFlag enfocándose en FontName
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();

            // Guarda el libro de trabajo
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


