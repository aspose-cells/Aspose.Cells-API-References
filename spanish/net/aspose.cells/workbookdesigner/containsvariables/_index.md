---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si la primera hoja de cálculo contiene variables personalizadas"
type: docs
url: /es/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Indica si la primera hoja de cálculo contiene variables personalizadas.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookDesigner.VariablesWorksheetName. Esta propiedad será eliminada 3 meses después, a partir de septiembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crear una instancia de WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Mostrar el valor actual de la propiedad ContainsVariables
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Establecer la propiedad ContainsVariables a true
                designer.ContainsVariables = true;

                // Mostrar el valor actualizado
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Guardar el resultado
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
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


