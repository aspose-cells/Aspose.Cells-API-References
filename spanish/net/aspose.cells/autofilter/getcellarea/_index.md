---
title: "AutoFilter.GetCellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Obtiene el CellArea donde se aplica este AutoFilter"
type: docs
url: /es/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Obtiene el [`CellArea`](../../cellarea/) donde se aplica este AutoFilter.

```csharp
public CellArea GetCellArea()
```

### Valor de retorno

el área a la que se aplica este filtro

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar datos de muestra para la demostración de AutoFilter
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Aplicar AutoFilter a los encabezados (índice de fila 0) cubriendo las columnas A-C (0-2)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // Obtener el CellArea donde se aplica AutoFilter
                CellArea result = autoFilter.GetCellArea();

                // Mostrar las coordenadas del rango de AutoFilter
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // Aplicar un filtro simple para demostrar la funcionalidad (opcional)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Guardar el libro con AutoFilter aplicado
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Obtiene el [`CellArea`](../../cellarea/) donde se aplica el AutoFilter especificado.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| refreshAppliedRange | Booleano | Indica si se debe refrescar el rango aplicado. Para el rango aplicado del auto filter, la última fila puede cambiar cuando los datos de las celdas cambian. Si este indicador es verdadero, entonces la última fila del rango se recalculará según los datos actuales de las celdas. |

### Valor de retorno

el área a la que se aplica este filtro

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos de muestra para AutoFilter
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // Establecer el rango de AutoFilter (fila 0 a 3, columna 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // Llamar a GetCellArea con refreshAppliedRange=true
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // Mostrar el rango aplicado del AutoFilter
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


