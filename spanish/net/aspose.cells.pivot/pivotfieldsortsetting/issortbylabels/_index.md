---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. Indica si se debe ordenar el campo por sí mismo o por el campo de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

Indica si se debe ordenar el campo por sí mismo o por el campo de datos.

```csharp
public bool IsSortByLabels { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtener la configuración de ordenación del campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Mostrar valor actual de IsSortByLabels
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // Nota: IsSortByLabels es de solo lectura, por lo que no podemos establecerlo directamente
            // En su lugar, demostraremos su significado examinando la configuración de ordenación

            // Mostrar propiedades de ordenación relacionadas
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


