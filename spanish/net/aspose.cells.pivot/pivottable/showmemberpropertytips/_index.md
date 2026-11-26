---
title: "PivotTable.ShowMemberPropertyTips"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica un valor booleano que indica si la información de la propiedad del miembro debe omitirse de los tooltips de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showmemberpropertytips/
---
## PivotTable.ShowMemberPropertyTips property

Especifica un valor booleano que indica si la información de propiedades de los miembros debe omitirse de las descripciones emergentes de la tabla dinámica.

```csharp
public bool ShowMemberPropertyTips { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowMemberPropertyTipsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de ShowMemberPropertyTips
            Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);

            // Cambiar la propiedad ShowMemberPropertyTips
            pivotTable.ShowMemberPropertyTips = false;
            Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);

            // Calcular datos y actualizar la tabla dinámica
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


