---
title: "DataModelTable.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModelTable. Obtiene el id de la tabla del modelo de datos"
type: docs
url: /es/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Obtiene el id de la tabla del modelo de datos.

```csharp
public string Id { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Crear un ListObject (tabla)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Obtener el DataModelTable (esto es solo lectura en el libro de trabajo)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Mostrar el valor actual del Id
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Nota: la propiedad Id es de solo lectura, por lo que no podemos establecerla
            // Esto demuestra cómo acceder y usar el Id existente

            // Ejemplo de uso: comparar los IDs de tabla al trabajar con múltiples tablas
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


