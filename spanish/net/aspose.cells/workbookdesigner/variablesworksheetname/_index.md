---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WorkbookDesigner. Obtiene y establece el nombre de la hoja de cálculo que contiene el smart marker de variables"
type: docs
url: /es/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Obtiene y establece el nombre de la hoja de cálculo que contiene variables smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();

                // Agrega una hoja de cálculo llamada "Variables" para demostrar la propiedad
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Crear una instancia de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Muestra el valor actual de VariablesWorksheetName
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Establece un nuevo valor para VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Agrega otra hoja de cálculo con marcadores inteligentes
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Procesa los marcadores inteligentes
                designer.Process();

                // Guarda el libro de trabajo
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


