---
title: "PivotTableCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTableCollection. Elimina la PivotTable en el índice especificado y elimina los datos de la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Elimina la PivotTable en el índice especificado y elimina los datos de la PivotTable

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice de posición en la colección PivotTable |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Agregar múltiples pivot tables
            sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");

            // Eliminar tabla dinámica en el índice 1 (segunda tabla dinámica)
            sheet.PivotTables.RemoveAt(1);

            // Verificar el recuento después de la eliminación
            Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Borra la PivotTable en el índice especificado

```csharp
public void RemoveAt(int index, bool keepData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice de posición en la colección PivotTable |
| keepData | Booleano | Indica si se deben conservar los datos de la PivotTable |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demostrar RemoveAt con keepData=true
            worksheet.PivotTables.RemoveAt(0, true);
            Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);

            // Agregar otra tabla dinámica
            index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demostrar RemoveAt con keepData=false
            worksheet.PivotTables.RemoveAt(0, false);
            Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


