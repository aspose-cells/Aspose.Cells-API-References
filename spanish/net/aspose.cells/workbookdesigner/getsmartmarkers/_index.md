---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookDesigner. Devuelve una colección de marcadores inteligentes en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Devuelve una colección de marcadores inteligentes en una hoja de cálculo.

```csharp
public string[] GetSmartMarkers()
```

### Valor de retorno

Una colección de marcadores inteligentes

### Observaciones

Se crea una matriz de cadenas en cada llamada. La matriz se ordena y se eliminan los valores duplicados.

### Ejemplos

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Crear un archivo de plantilla de ejemplo en memoria
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Agregar marcadores inteligentes a la plantilla
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Guardar plantilla en flujo de memoria
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Inicializar WorkbookDesigner con la plantilla
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Obtener y mostrar marcadores inteligentes
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Preparar origen de datos
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Establecer origen de datos y procesar
            designer.SetDataSource(data);
            designer.Process();
            
            // Guardar resultado
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


