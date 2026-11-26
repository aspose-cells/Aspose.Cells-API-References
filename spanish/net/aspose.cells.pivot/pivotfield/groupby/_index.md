---
title: "PivotField.GroupBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Agrupa automáticamente el campo con intervalo"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Agrupa automáticamente el campo con intervalo

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intervalo | Double | El interno del grupo. Se asignará un valor automático si es cero, |
| newField | Booleano | Indica si se está añadiendo un nuevo campo a la tabla dinámica. Solo para el agrupamiento DateTime. |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Añade el campo al área de columnas
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Agrupa el campo por 1 (intervalo) con rango automático
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Agrupa automáticamente el campo con interno

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| grupos | PivotGroupByType[] | Tipos de agrupación |
| intervalo | Double | El interno del grupo. Se asignará un valor automático si es cero, solo funciona para agrupar por Números o Días. |
| newField | Booleano | Indica si se está añadiendo un nuevo campo a la tabla dinámica. |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Agrupa el archivo por los tipos de grupo de fecha.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha y hora de inicio |
| fin | DateTime | La fecha y hora de fin |
| grupos | PivotGroupByType[] | Tipos de agrupación |
| intervalo | Double | El intervalo |
| firstAsNewField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica. Solo para el primer elemento del grupo. |

### Valor de retorno

Falso significa que este campo no pudo agruparse por fecha y hora.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con fechas para la tabla dinámica
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            // Preparar parámetros para el método GroupBy
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Llamar al método GroupBy con parámetros de fecha
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Actualizar tabla dinámica
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Agrupa el archivo por los tipos de grupo de fecha.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoStart | Booleano | Indica si se debe detectar automáticamente el valor de fecha y hora de inicio. |
| inicio | DateTime | La fecha y hora de inicio |
| isAutoEnd | Booleano | Indica si se debe detectar automáticamente el valor de fecha y hora de fin. |
| fin | DateTime | La fecha y hora de fin |
| grupos | PivotGroupByType[] | Tipos de agrupación |
| intervalo | Double | El intervalo |
| firstAsNewField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica. Solo para el primer elemento del grupo. |

### Valor de retorno

Falso significa que este campo no pudo agruparse por fecha y hora.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Agrupa el archivo por número.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | Double | El valor de inicio |
| fin | Double | El valor final |
| intervalo | Double | El intervalo |
| newField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica |

### Valor de retorno

Falso significa que este campo no pudo agruparse por fecha y hora.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila y agruparlo
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Guarda el libro de trabajo
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Agrupa el archivo por número.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAutoStart | Booleano | Indica si se debe detectar automáticamente el valor de inicio. |
| inicio | Double | El valor de inicio |
| isAutoEnd | Booleano | Indica si se debe detectar automáticamente el valor final. |
| fin | Double | El valor final |
| intervalo | Double | El intervalo |
| newField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica |

### Valor de retorno

Falso significa que este campo no pudo agruparse por fecha y hora.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método PivotField.Group(PivotFieldGroupOptions). Este método será eliminado 6 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Agrupar el campo de forma personalizada.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Los elementos de grupo personalizados. |
| newField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica |

### Valor de retorno

Falso significa que este campo no pudo agruparse por fecha y hora.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions options) con la propiedad PivotFieldGroupOptions.DiscreteGroupItems. Este método será eliminado 6 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            // Crear elementos de grupo personalizados
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Llamar al método GroupBy con elementos de grupo personalizados
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Actualizar tabla dinámica
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Agrupar el campo de forma personalizada.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Los elementos de grupo personalizados. |
| newField | Booleano | Indica si se agrega un nuevo campo a la tabla dinámica |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotField.Group(PivotFieldGroupOptions options) con la propiedad PivotFieldGroupOptions.DiscreteGroupItems. Este método será eliminado 6 meses después, a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


