---
title: "Clase DataModel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DataModels.DataModel clase. Representa el modelo de datos"
type: docs
url: /es/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Representa el modelo de datos.

```csharp
public class DataModel
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Obtiene todas las relaciones de las tablas en el modelo de datos. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Obtiene todas las tablas en el modelo de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenga el DataModel del libro de trabajo en lugar de crear una nueva instancia
            DataModel dataModel = workbook.DataModel;

            // Demostrar el acceso a tablas y relaciones (propiedades de solo lectura)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Nota: Dado que Tablas y Relaciones son colecciones de solo lectura,
            // solo podemos acceder a los elementos existentes pero no modificarlos directamente

            // Guardar el libro de trabajo (DataModel se usa típicamente internamente por Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


