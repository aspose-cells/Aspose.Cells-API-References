---
title: "ListObject.DataRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Obtiene el rango de datos de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Obtiene el rango de datos de la Tabla.

```csharp
public Range DataRange { get; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataRangeDemo
    {
        public static void Run()
        {
            Encoding.RegisterProvider(CodePagesEncodingProvider.Instance);
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crear un ListObject (Tabla)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Obtener el rango de datos de la tabla
            Aspose.Cells.Range dataRange = table.DataRange;

            // Demostrar el uso de DataRange
            Console.WriteLine("Table Data Range: " + dataRange.Address);
            Console.WriteLine("Row Count: " + dataRange.RowCount);
            Console.WriteLine("Column Count: " + dataRange.ColumnCount);

            // Agregar una fórmula a la última columna usando DataRange
            string formula = "=CONCATENATE(\"ID-\", [ID])";
            int lastColIndex = dataRange.ColumnCount - 1;
            dataRange[0, lastColIndex].PutValue("FormattedID");
            for (int i = 1; i < dataRange.RowCount; i++)
            {
                dataRange[i, lastColIndex].Formula = formula;
            }

            // Guarda el libro de trabajo
            workbook.Save("ListObjectDataRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


