---
title: "PivotField.SortBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Ordena este campo dinámico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Ordena este campo dinámico.

```csharp
public void SortBy(SortOrder sortType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | SortOrder | El tipo de ordenación de este campo. |

### Ver también

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Ordena este campo dinámico.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | SortOrder | El tipo de ordenación de este campo. |
| fieldSortedBy | Int32 | El índice del campo dinámico por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.SortBy(SortOrder, int,string) o la propiedad PivotField.IsAutoSort. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ordene el campo de fila en orden descendente con índice -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Ordena este campo dinámico.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | SortOrder | El tipo de ordenación de este campo. |
| fieldSortedBy | Int32 | El índice del campo dinámico por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |
| dataType | PivotLineType | El tipo de datos por los que se ordena. |
| cellName | String | Ordenar por valores en la fila o columna |

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.SortBy(SortOrder, int,string). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ordene el campo de fila
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Calcular datos
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Ordena este campo dinámico.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sortType | SortOrder | El tipo de ordenación de este campo. |
| fieldSortedBy | Int32 | El índice del campo dinámico por el cual se ordena. -1 significa ordenar por las etiquetas de datos de este campo, otros valores indican el índice del campo de datos por el cual se ordena. |
| cellName | String | Ordenar por valores en la fila o columna. Si es Null, agrupar por el total del campo; de lo contrario, agrupar por los valores en la columna o fila seleccionada. |

### Ver también

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


