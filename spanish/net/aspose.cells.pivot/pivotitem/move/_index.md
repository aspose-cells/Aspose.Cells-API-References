---
title: "PivotItem.Move"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotItem. Mueve el elemento hacia arriba o hacia abajo"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Mueve el elemento hacia arriba o hacia abajo

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desplazamiento | Int32 | El número de movimientos hacia arriba o hacia abajo. Mueve el elemento hacia arriba si esto es menor que cero; Mueve el elemento hacia abajo si esto es mayor que cero. |
| isSameParent | Booleano | Especifica si la operación de movimiento está en el mismo nodo padre o no |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice PivotTable.MoveItem(PivotFieldType, string[],bool,int) o el método PivotItem.Move(int) en su lugar. Este método será eliminado 12 meses después a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear datos de muestra para tabla dinámica
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Obtenga los elementos pivot y demuestre el método Move
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Mover el primer elemento a la posición 1 (segunda posición) con elementos secundarios
            items[0].Move(1, true);
            
            // Guarda el libro de trabajo
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Mueve el elemento hacia arriba o abajo en el campo pivot

```csharp
public void Move(int offset)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desplazamiento | Int32 | El número de movimientos hacia arriba o hacia abajo. Mueve el elemento hacia arriba si esto es menor que cero; Mueve el elemento hacia abajo si esto es mayor que cero. |

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


