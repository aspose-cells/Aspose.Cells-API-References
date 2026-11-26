---
title: "PivotAreaCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotAreaCollection. Añade un área de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotareacollection/add/
---
## Add(PivotArea) {#add}

Añade un área de tabla dinámica.

```csharp
[Obsolete("Use PivotAreaCollection.AddPivotArea(PivotArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(PivotArea pivotArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotArea | PivotArea | El área de tabla dinámica. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método AddPivotArea(). Este método será eliminado 6 meses después desde diciembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionMethodAddWithPivotAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar tabla dinámica
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Agregue campos a áreas pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Crear formato condicional
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // Cree un área de tabla dinámica y añádala a la colección
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Agregar condición de formato
            FormatCondition fc = pcf.FormatConditions[pcf.FormatConditions.AddCondition(FormatConditionType.CellValue)];
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Formula1 = "15";
            fc.Style.BackgroundColor = Color.Yellow;

            // Calcular datos y guardar
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotAreaCollectionMethodAddWithPivotAreaDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Agrega un área basada en la vista de la tabla dinámica.

```csharp
public void Add(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | El área basada en la vista de tabla dinámica. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Definir un área de celda para agregar a las áreas de tabla dinámica
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.StartColumn = 0;
            cellArea.EndRow = 2;
            cellArea.EndColumn = 1;

            // Obtener la colección de áreas de tabla dinámica seleccionando el área
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea);

            try
            {
                // Llamar al método Add con el parámetro CellArea
                pivotAreas.Add(cellArea);

                Console.WriteLine("Pivot area added successfully for cell area: " +
                    $"({cellArea.StartRow},{cellArea.StartColumn}) to ({cellArea.EndRow},{cellArea.EndColumn})");

                // Mostrar las áreas de tabla dinámica agregadas
                foreach (PivotArea area in pivotAreas)
                {
                    CellArea[] areas = area.GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Pivot area covers: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotAreaCollectionMethodAddWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


