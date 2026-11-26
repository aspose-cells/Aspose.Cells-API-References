---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de WorkbookDesigner. Inicializa una nueva instancia de la clase WorkbookDesigner"
type: docs
url: /es/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Inicializa una nueva instancia de la clase [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner()
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo WorkbookDesigner usando el constructor
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Crea una fuente de datos de ejemplo
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Crea un nuevo libro de trabajo y establécelo como el libro de trabajo del diseñador
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece marcadores en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Asigna el libro de trabajo al diseñador
            designer.Workbook = workbook;

            // Establecer origen de datos y procesar
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Guardar el resultado
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    public class Level
    {
        public string Name { get; set; }
        public string Value { get; set; }

        public Level(string name, string value)
        {
            Name = name;
            Value = value;
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Inicializa una nueva instancia de la clase [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| libro de trabajo | Libro de trabajo | El archivo de libro de trabajo de plantilla. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece datos de ejemplo en las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // Crear fuente de datos JSON
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // Inicializa WorkbookDesigner con el libro de trabajo
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // Establece la fuente de datos JSON
            designer.SetJsonDataSource("ds", jsonData);
            
            // Procesar el diseñador
            designer.Process();
            
            // Mostrar el resultado
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


