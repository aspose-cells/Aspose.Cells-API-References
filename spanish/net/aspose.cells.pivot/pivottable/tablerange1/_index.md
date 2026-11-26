---
title: "PivotTable.TableRange1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Devuelve un objeto CellArea que representa el rango que contiene todo el informe de PivotTable pero no incluye los campos de página. Solo lectura"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/tablerange1/
---
## PivotTable.TableRange1 property

Devuelve un objeto CellArea que representa el rango que contiene todo el informe de la tabla dinámica, pero no incluye los campos de página. Solo lectura.

```csharp
public CellArea TableRange1 { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange1Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo con datos de ejemplo
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Crear una tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            
            // Agregar campos a la tabla dinámica
            int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Configurar tabla dinámica
            pivotTable.ShowInTabularForm();
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demostrar la propiedad TableRange1
            Console.WriteLine("Pivot Table Range:");
            Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
            Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
            Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
            Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


