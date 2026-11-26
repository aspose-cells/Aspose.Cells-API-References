---
title: "ListObject.ConvertToRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObject. Convertir la tabla a rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Convierte la tabla a rango.

```csharp
public void ConvertToRange()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("John");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Mary");
            
            // Crear un objeto de lista
            int index = sheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = sheet.ListObjects[index];
            
            Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
            
            // Convertir el objeto de lista a rango
            listObject.ConvertToRange();
            
            Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectConversion.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Convierte la tabla a rango.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | TableToRangeOptions | las opciones al convertir la tabla a rango. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeWithTableToRangeOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
                for (int row = 1; row < 5; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Crear tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Convertir tabla a rango con opciones
            TableToRangeOptions options = new TableToRangeOptions();
            options.LastRow = 4;
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithOptions.xlsx");
        }
    }
}
```

### Ver también

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


