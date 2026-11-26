---
title: "WorkbookDesigner.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Obtiene y establece el objeto Workbook"
type: docs
url: /es/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Obtiene y establece el objeto `Workbook`.

```csharp
public Workbook Workbook { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person1
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person1(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crear un nuevo diseñador de libros de trabajo
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Establecer la propiedad workbook con un nuevo libro de trabajo
            designer.Workbook = new Workbook();
            
            // Agregar una hoja de cálculo y algunos marcadores de plantilla
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Crear origen de datos
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Establecer origen de datos y procesar
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Mostrar resultados
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Guarda el libro de trabajo
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


