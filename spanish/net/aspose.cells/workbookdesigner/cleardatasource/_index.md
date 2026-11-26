---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookDesigner. Elimina todas las fuentes de datos"
type: docs
url: /es/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Borra todas las fuentes de datos.

```csharp
public void ClearDataSource()
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerMethodClearDataSourceDemo
    {
        public static void Run()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Worksheet worksheet = designer.Workbook.Worksheets[0];

            // Crear datos de ejemplo
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Configurar marcadores inteligentes
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Primer enlace de datos
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Eliminar la fuente de datos y volver a enlazar
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Guardar el resultado
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


