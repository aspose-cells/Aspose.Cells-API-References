---
title: "ExternalConnection.ClassType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene el tipo de este objeto ExternalConnection"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Obtiene el tipo de este objeto [`ExternalConnection`](../).

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Crear una tabla dinámica con conexión Data Model
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtener la conexión externa y demostrar la propiedad ClassType
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // Guarda el libro de trabajo
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


