---
title: "PivotTableCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTableCollection. Obtiene el informe de PivotTable por índice"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Obtiene el informe de PivotTable por índice.

```csharp
public PivotTable this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de tablas dinámicas
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Acceder a la primera tabla dinámica usando la propiedad Item (indexador)
            PivotTable pivotTable = pivotTables[0];
            
            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();
            
            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
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

## PivotTableCollection indexer (2 of 3)

Obtiene el informe de PivotTable por el nombre de la tabla dinámica.

```csharp
public PivotTable this[string name] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurar tabla dinámica usando la propiedad Item
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Acceder a la tabla dinámica usando la propiedad Item
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Modificar datos y actualizar
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Guarda el libro de trabajo
            workbook.Save("PivotTableDemo.xlsx");
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

## PivotTableCollection indexer (3 of 3)

Obtiene la [`PivotTable`](../../pivottable/) ubicada en la celda.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Agregar una tabla dinámica a la hoja de cálculo
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Acceder a la PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Demostrar el acceso a una tabla dinámica usando la propiedad Item (indexador)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Demostrar el acceso por nombre usando la propiedad Item
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // Configura la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Actualizar y calcular datos
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Guarda el libro de trabajo
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
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


