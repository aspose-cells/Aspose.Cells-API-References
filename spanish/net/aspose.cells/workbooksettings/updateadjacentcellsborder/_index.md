---
title: "WorkbookSettings.UpdateAdjacentCellsBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Indica si se actualiza el borde de celdas adyacentes"
type: docs
url: /es/net/aspose.cells/workbooksettings/updateadjacentcellsborder/
---
## WorkbookSettings.UpdateAdjacentCellsBorder property

Indica si se actualiza el borde de las celdas adyacentes.

```csharp
public bool UpdateAdjacentCellsBorder { get; set; }
```

### Observaciones

El valor predeterminado es falso. Por ejemplo: el borde inferior de la celda A1 se actualiza, el borde superior de la celda A2 también debe cambiarse.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateAdjacentCellsBorderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Habilitar la actualización de los bordes de las celdas adyacentes
            workbook.Settings.UpdateAdjacentCellsBorder = true;

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el valor y aplicar un borde a la celda A1
            worksheet.Cells["A1"].PutValue("Sample");
            Style styleA1 = workbook.CreateStyle();
            styleA1.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            styleA1.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            worksheet.Cells["A1"].SetStyle(styleA1);

            // Establecer el valor en la celda adyacente B1 (a la derecha de A1)
            worksheet.Cells["B1"].PutValue("Adjacent");

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            Console.WriteLine("Workbook saved with adjacent cell border update enabled.");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


