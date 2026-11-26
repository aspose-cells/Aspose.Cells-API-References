---
title: "PivotTableCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTableCollection. Agrega una nueva tabla dinámica moderna desde Excel 2007 en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Agrega un nuevo PivotTable moderno (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1!A1:C8 |
| cellName | String | El nombre de la celda de la esquina superior izquierda para el destino de la tabla dinámica. |

### Valor de retorno

La instancia de tabla dinámica recién creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Agrega un nuevo PivotTable moderno (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1!A1:C8 |
| cellName | String | El nombre de la celda de la esquina superior izquierda para el destino de la tabla dinámica. |
| opciones | PivotTableCreateOptions | Las opciones para crear la tabla dinámica. |

### Valor de retorno

La instancia de tabla dinámica recién creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Agrega un nuevo PivotTable moderno (desde Excel 2007) en la fila y columna especificadas de la hoja de cálculo con opciones predeterminadas.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1!A1:C8 |
| fila | Int32 | El índice de fila basado en cero de la esquina superior izquierda para el destino de la tabla dinámica. |
| columna | Int32 | El índice de columna basado en cero de la esquina superior izquierda para el destino de la tabla dinámica. |

### Valor de retorno

La instancia de tabla dinámica recién creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Agrega un nuevo PivotTable en la fila y columna especificadas de la hoja de cálculo.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1!A1:C8 |
| fila | Int32 | El índice de fila basado en cero de la esquina superior izquierda para el destino de la tabla dinámica. |
| columna | Int32 | El índice de columna basado en cero de la esquina superior izquierda para el destino de la tabla dinámica. |
| opciones | PivotTableCreateOptions | Opciones de creación de tabla dinámica. |

### Valor de retorno

La instancia de tabla dinámica recién creada.

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | Los datos para la caché de la nueva tabla dinámica. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice en esta lista de tablas dinámicas.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del CSV de origen
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Agregar datos de ejemplo
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // Crear hoja de cálculo de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Obtener el rango de datos de origen
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // Agregar tabla dinámica usando parámetros String, String, String
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // Configurar tabla dinámica
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | Los datos para la caché de la nueva tabla dinámica. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |
| useSameSource | Booleano | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

### Valor de retorno

El índice de la caché recién añadida.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Definir parámetros para el método Add
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Llamar al método Add con los parámetros (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Configura la tabla dinámica
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice en esta lista de tablas dinámicas.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo para datos
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Agregar datos de ejemplo
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Agregar una hoja de cálculo para tabla dinámica
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar tabla dinámica usando el método Add con parámetros (String, Int32, Int32, String)
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Acceder a la tabla dinámica
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Establecer función de consolidación
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe PivotTable. |
| useSameSource | Booleano | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

### Valor de retorno

El índice de la caché recién añadida.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de septiembre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Definir el rango de datos
            string sourceData = "A1:C4";
            
            try
            {
                // Llamar al método Add con los parámetros: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Acceder a la tabla dinámica recién creada
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configurar tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Agrega una nueva tabla dinámica con el diseño y estilo heredados de Excel 97-2003.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva PivotTable. Ejemplo: Sheet1!A1:C8 |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe PivotTable. |
| useSameSource | Booleano | Indica si se utiliza la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |
| isXlsClassic | Booleano | Indica si se agrega una tabla dinámica clásica de Excel 97-2003. |

### Valor de retorno

El índice de la caché recién añadida.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de octubre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Definir el rango de datos de origen
            string sourceData = "A1:C5";

            try
            {
                // Llame al método Add con los parámetros (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Configura la tabla dinámica
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Agrega una nueva PivotTable.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva PivotTable. Ejemplo: Sheet1!A1:C8 |
| celda | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |
| useSameSource | Booleano | Indica si se está usando la misma fuente de datos cuando otra tabla dinámica existente ha utilizado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria cuando la misma fuente de datos se haya reunido en una única caché de pivot table. |
| isXlsClassic | Booleano | Indica si se agrega una tabla dinámica clásica de Excel 97-2003. |

### Valor de retorno

El índice de la caché recién añadida.

### Observaciones

NOTA: Este método está obsoleto. Es equivalente a llamar a PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Por favor, use la sobrecarga PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) en su lugar. Este método será eliminado 12 meses después de octubre de 2026. Disculpe cualquier inconveniente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene datos de ejemplo
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // Agregar pivot table con los parámetros especificados
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Agrega un nuevo PivotTable basado en otro PivotTable.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | La pivotTable de origen. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la PivotTable recién añadida.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crear una pivot table a partir del rango de datos
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Llame al método Add con los parámetros (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
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

## Add(PivotTable, int, int, string) {#add_4}

Agrega un nuevo PivotTable basado en otro PivotTable.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | La pivotTable de origen. |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la PivotTable recién añadida.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crear una pivot table de origen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Llame al método Add con los parámetros (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
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

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Agrega un nuevo objeto PivotTable a la colección con múltiples rangos de consolidación como fuente de datos.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String[] | Los rangos de consolidación múltiple, como {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Booleano | Indica si se crea automáticamente un campo de página único. Si es verdadero, el siguiente parámetro pageFields será ignorado. |
| pageFields | PivotPageFields | Los elementos del campo de página pivot. |
| destCellName | String | destCellName El nombre del nuevo informe de PivotTable. |
| tableName | String | el nombre del nuevo informe de PivotTable. |

### Valor de retorno

El índice de la PivotTable recién añadida.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Definir rango de datos
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Llame al método Add con los parámetros especificados
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Acceder a la tabla dinámica recién creada
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Configurar campos de la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Agrega un nuevo objeto PivotTable a la colección con múltiples rangos de consolidación como fuente de datos.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String[] | Los rangos de consolidación múltiple, como {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Booleano | Indica si se crea automáticamente un campo de página único. Si es verdadero, el siguiente parámetro pageFields será ignorado |
| pageFields | PivotPageFields | Los elementos del campo de página pivot. |
| fila | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| columna | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la PivotTable recién añadida.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Definir parámetros para el método Add
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Llame al método Add con los parámetros especificados
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Configura la tabla dinámica
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Actualizar datos
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


