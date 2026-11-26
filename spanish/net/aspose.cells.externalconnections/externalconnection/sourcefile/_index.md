---
title: "ExternalConnection.SourceFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Se utiliza cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación URI o en la ruta de archivo específica del sistema."
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Se utiliza cuando la fuente de datos externa es basada en archivos. Cuando una conexión a dicha fuente de datos falla, la aplicación de hoja de cálculo intenta conectarse directamente a este archivo. Puede expresarse en notación URI o ruta de archivo específica del sistema.

```csharp
public string SourceFile { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceFileDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (!string.IsNullOrEmpty(connection.SourceFile))
                    connection.SourceFile = connection.SourceFile.Replace("C:\\", "D:\\");
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


