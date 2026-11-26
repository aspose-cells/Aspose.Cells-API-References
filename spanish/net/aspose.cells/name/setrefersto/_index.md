---
title: "Name.SetRefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Name. Establezca la referencia de este Name"
type: docs
url: /es/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Establezca la referencia de este Name.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| refersTo | String | La referencia. |
| isR1C1 | Booleano | Indica si la referencia está en formato R1C1. |
| isLocal | Booleano | Indica si la referencia está formateada según la configuración regional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // Llame a SetRefersTo con parámetros (String, Boolean, Boolean)
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Mostrar el resultado
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Verificar usando el rango con nombre en una fórmula
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


