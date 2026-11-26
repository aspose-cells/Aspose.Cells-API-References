---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de WorkbookDesigner. Establece el valor de cadena JSON como fuente de datos de los marcadores inteligentes"
type: docs
url: /es/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Establece el valor de cadena JSON como fuente de datos de los marcadores inteligentes.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la tabla. Si el valor de JSON representa un objeto, podría ser nulo. |
| json | String | El valor de la cadena Json. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega un marcador de ejemplo en la celda A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Crear diseñador de libros de trabajo
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Datos JSON de ejemplo
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Establece la fuente de datos JSON
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Procesa los marcadores
            designer.Process();
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


