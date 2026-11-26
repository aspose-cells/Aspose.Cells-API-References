---
title: "PivotField.ShowValuesAs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Muestra los valores del campo de datos en un formato de visualización diferente cuando se utiliza el cálculo ShowDataAs"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Muestra los valores del campo de datos en un formato de visualización diferente cuando se utiliza el cálculo ShowDataAs.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | El tipo de formato de visualización de datos. |
| baseField | Int32 | El índice al campo en el que se basa el cálculo ShowDataAs. |
| baseItemPositionType | PivotItemPositionType | El tipo de posición del elemento base. |
| baseItem | Int32 | El índice al elemento base en el que se basa el cálculo ShowDataAs. Solo funciona cuando baseItemPositionType es personalizado. |

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice el método PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campo de fila
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Agregar campo de columna
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Agregar campo de datos y configurar ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Calcular datos y guardar
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Establece el cálculo "Mostrar valores como" para este campo de tabla dinámica.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Tipo del cálculo "Show Values As". |
| baseField | Int32 | Índice del campo base utilizado para el cálculo. |
| baseItem | Int32 | Índice del elemento base para el cálculo. Use [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) para el elemento anterior, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) para el elemento siguiente; los valores no negativos denotan el índice ordinal de un elemento pivot específico. |

### Observaciones

Solo para campo de datos.

### Ver también

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Configura el cálculo "Mostrar valores como" para este campo de datos.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | El tipo de cálculo para Show Values As. |
| baseField | String | El nombre del campo base utilizado en el cálculo. |
| baseItem | String | Título de un elemento pivot regular. También acepta palabras clave literales reservadas: `(previous)` para el elemento anterior, `(next)` para el elemento siguiente. Pase `null` si el tipo de cálculo seleccionado no requiere un elemento base. |

### Ver también

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


