---
title: "PivotTable.GetChildren"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Obtiene las tablas dinámicas hijas que utilizan estos datos de PivotTable como fuente de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Obtiene las tablas dinámicas secundarias que utilizan estos datos de tabla dinámica como fuente de datos.

```csharp
[Obsolete("Use PivotTable.GetDependentPivotTables() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotTable[] GetChildren()
```

### Valor de retorno

el objeto de matriz PivotTable

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.GetDependentPivotTables(). Este método será eliminado 12 meses después de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetChildrenDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Crear tabla dinámica principal
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
            PivotTable mainPivotTable = pivotTables[index];
            mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crear tabla dinámica secundaria
            index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
            PivotTable childPivotTable = pivotTables[index];
            childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Establecer relación compartiendo campos base
            foreach (PivotField field in mainPivotTable.BaseFields)
            {
                childPivotTable.BaseFields.Add(field);
            }

            // Demostrar el método GetChildren()
            Console.WriteLine("Child Pivot Tables:");
            foreach (PivotTable child in mainPivotTable.GetChildren())
            {
                Console.WriteLine("Child Pivot Table Name: " + child.Name);
                Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
            }
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


