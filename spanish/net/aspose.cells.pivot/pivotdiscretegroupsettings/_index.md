---
title: "Clase PivotDiscreteGroupSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotDiscreteGroupSettings clase. Representa el grupo discreto del campo de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotdiscretegroupsettings/
---
## PivotDiscreteGroupSettings class

Representa el grupo discreto del campo de tabla dinámica.

```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DiscreteItems](../../aspose.cells.pivot/pivotdiscretegroupsettings/discreteitems/) { get; } | Obtiene los elementos discretos. |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | (**Obsoleto.**) Obtiene los elementos discretos. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Obtiene el tipo de grupo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsDemo
    {
        public static void PivotDiscreteGroupSettingsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregando algunos datos de muestra
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Quantity");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(15);
            worksheet.Cells[3, 0].PutValue("A");
            worksheet.Cells[3, 1].PutValue(10);
            worksheet.Cells[4, 0].PutValue("B");
            worksheet.Cells[4, 1].PutValue(15);

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Establece los campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accediendo al campo de fila
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);

            // Crear una instancia de PivotDiscreteGroupSettings
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Establecer el tipo de grupo a Discrete (Esta propiedad es de solo lectura)
            // Mostrar el tipo de grupo actual
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Guarda el libro de trabajo
            workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


