---
title: "PivotField.CurrentPageItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene o establece el elemento de página actualmente mostrado solo para este campo de página de pivote."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Obtiene o establece el elemento de página actualmente mostrado para este campo de tabla dinámica (solo campo de página).

```csharp
public short CurrentPageItem { get; set; }
```

### Observaciones

Utilice [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) como el valor centinela para indicar "Seleccionar todo". Este es un marcador predefinido y no es un índice de elemento válido.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Actualizar datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtener campos de página
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Mostrar elementos de página actuales
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Cambiar el elemento de página actual
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


