---
title: "PivotDiscreteGroupSettings.Items"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotDiscreteGroupSettings. Obtiene los elementos discretos"
type: docs
url: /es/net/aspose.cells.pivot/pivotdiscretegroupsettings/items/
---
## PivotDiscreteGroupSettings.Items property

Obtiene los elementos discretos.

```csharp
[Obsolete("Use PivotField.GroupBy(DiscreteGroupItem[], bool) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomPiovtFieldGroupItem[] Items { get; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.GroupBy(DiscreteGroupItem[], bool). Este método será eliminado 12 meses después desde julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsPropertyItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Apple");
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(150);
            worksheet.Cells["B6"].PutValue(250);

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Obtener el campo de tabla dinámica y agruparlo
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);

            // Acceder a la configuración del grupo discreto
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Mostrar los elementos actuales
            Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
            foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
            {
                Console.WriteLine("Item: " + item.ToString());
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


