---
title: "PivotTableCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTableCollection. Elimina la PivotTable especificada y elimina los datos de la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Elimina el PivotTable especificado y elimina los datos del PivotTable

```csharp
public void Remove(PivotTable pivotTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | Objeto PivotTable |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtener colección de tablas dinámicas
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Comprobar si hay alguna tabla dinámica
            if (pivotTables.Count > 0)
            {
                // Obtener la primera tabla dinámica
                PivotTable pivotTable = pivotTables[0];
                
                // Eliminar la tabla dinámica
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Elimina el PivotTable especificado

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | Objeto PivotTable |
| keepData | Booleano | Indica si se deben conservar los datos de la PivotTable |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demostrar el método Remove con PivotTable y parámetros booleanos
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Eliminar tabla dinámica pero conservar los datos (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Agregar otra tabla dinámica
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Eliminar tabla dinámica y borrar los datos (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


