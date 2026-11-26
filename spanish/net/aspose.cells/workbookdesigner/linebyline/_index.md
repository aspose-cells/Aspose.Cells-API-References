---
title: "WorkbookDesigner.LineByLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si el procesamiento del marcador inteligente se realiza línea por línea"
type: docs
url: /es/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Indica si el procesamiento del marcador inteligente se realiza línea por línea.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Observaciones

El valor predeterminado es true. Si es False, el archivo de plantilla debe contener un rango llamado "_CellsSmartMarkers".

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice marcadores inteligentes de rango. Esta propiedad será eliminada 12 meses después, a partir de julio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con marcadores inteligentes
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Configurar marcadores inteligentes en la hoja de cálculo
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Crear datos de ejemplo
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Procesar con LineByLine establecido en false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Guardar el resultado
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Clase de datos simple para demostración
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


