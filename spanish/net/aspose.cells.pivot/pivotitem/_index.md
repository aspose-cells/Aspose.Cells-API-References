---
title: "Clase PivotItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotItem. Representa un elemento en un informe de PivotField."
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Representa un elemento en un informe de PivotField.

```csharp
public class PivotItem
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsoleto.**) Obtiene el índice del elemento pivot en el campo de caché. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Indica si este elemento pivot es un elemento de fórmula calculada. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Obtiene y establece si el detalle de este elemento pivot está oculto. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsoleto.**) Indica si este elemento pivot es un elemento de fórmula calculada. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Obtiene y establece si el elemento pivot está oculto. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsoleto.**) Obtiene y establece si el elemento pivot oculta el detalle. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Indica si el elemento fue eliminado de la fuente de datos. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Obtiene el nombre del elemento pivot. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Especifica el índice de este elemento en todos los PivotItems del campo. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsoleto.**) Especifica el índice de posición en los PivotItems bajo el mismo nodo padre. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Obtiene el valor del elemento pivot |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Obtiene el valor de fecha y hora del elemento pivot. Si el valor es nulo, devolverá DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Obtiene el valor doble del elemento pivot. Si el valor es nulo o no es un número, devolverá 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Obtiene la fórmula de este elemento calculado. Solo funciona cuando este elemento es calculado. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Obtiene el valor de cadena del elemento pivot. Si el valor es nulo, devolverá "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Mueve el elemento hacia arriba o abajo en el campo pivot |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsoleto.**) Mueve el elemento hacia arriba o abajo |

## Campos

| Nombre | Descripción |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Índice centinela de selección total de elementos de página (0x7FFD, no es un índice válido) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accede a los elementos pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Imprime el nombre del elemento pivot
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Establecer propiedades
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Imprime el valor del elemento pivot
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Usa métodos
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


