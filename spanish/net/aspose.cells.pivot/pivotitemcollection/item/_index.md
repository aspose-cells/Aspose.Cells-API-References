---
title: "PivotItemCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItemCollection. Obtiene el objeto PivotItem en el índice específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Obtiene el objeto PivotItem en el índice específico.

```csharp
public PivotItem this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;
            
            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Acceda a los elementos pivot mediante la propiedad Item
            PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
            
            // Demostrar el uso de la propiedad Item
            Console.WriteLine("First pivot item: " + pivotItems[0].Name);
            Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
            Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
        }
    }
}
```

### Ver también

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Obtiene el [`PivotItem`](../../pivotitem/) por el nombre específico.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Agregar una nueva hoja de cálculo para la tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Agregar tabla dinámica
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configurar tabla dinámica
            pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demuestra el uso de la propiedad Item y operaciones de movimiento
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Acceda a los elementos mediante la propiedad Item
            items["4H12"].Move(0, true);
            items["DIF400"].Move(-1, true);
            
            pivotTable.CalculateData();
            
            items["CA32"].Move(0, true);
            items["AAA3"].Move(-1, true);

            // Guarda el libro de trabajo
            workbook.Save("PivotItemCollectionDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


