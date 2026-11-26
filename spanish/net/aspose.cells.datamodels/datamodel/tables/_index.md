---
title: "DataModel.Tables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataModel. Obtiene todas las tablas en el modelo de datos"
type: docs
url: /es/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Obtiene todas las tablas en el modelo de datos.

```csharp
public DataModelTableCollection Tables { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder al modelo de datos
            DataModel dataModel = wb.DataModel;
            
            // Obtener la colección de tablas y mostrar el recuento
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Cargar libro de ejemplo con modelo de datos
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Acceder a la colección de tablas
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Iterar a través de las tablas
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### Ver también

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


