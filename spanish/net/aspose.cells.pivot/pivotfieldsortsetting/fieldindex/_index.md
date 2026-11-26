---
title: "PivotFieldSortSetting.FieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldSortSetting. Representa el índice del campo por el cual se ordena. 1 significa ordenar el PivotField por las etiquetas; otros valores significan ordenar por el campo de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldsortsetting/fieldindex/
---
## PivotFieldSortSetting.FieldIndex property

Representa el índice del campo por el cual se ordena. -1 significa ordenar el PivotField por las etiquetas; otros valores significan ordenar por el campo de datos.

```csharp
[Obsolete("Use PivotFieldSortSetting.SortBy property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int FieldIndex { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotFieldSortSetting.SortBy. Este método será eliminado 12 meses después a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtener la configuración de ordenación del campo pivot
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;

            // Mostrar el valor actual de FieldIndex
            Console.WriteLine("Current FieldIndex value: " + sortSetting.FieldIndex);

            // Nota: FieldIndex es de solo lectura y PivotFieldSortSetting no puede instanciarse directamente
            // ya que no tiene un constructor público. Solo podemos trabajar con la instancia existente
            // obtenida de la propiedad SortSetting del campo pivot.

            // Actualizar la tabla dinámica para aplicar los cambios
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guardar el resultado
            workbook.Save("PivotFieldSortSettingFieldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


