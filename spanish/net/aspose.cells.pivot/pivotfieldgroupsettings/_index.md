---
title: "Clase PivotFieldGroupSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotFieldGroupSettings. Representa la configuración de grupo del campo pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

Representa la configuración de grupo del campo de tabla dinámica.

```csharp
public class PivotFieldGroupSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | Obtiene el tipo de grupo del campo pivot. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Acceder al campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // Acceder a la configuración de grupo del campo de fila
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Mostrar el tipo de grupo del campo pivot
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


