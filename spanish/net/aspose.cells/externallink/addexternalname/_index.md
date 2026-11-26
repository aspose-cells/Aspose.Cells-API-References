---
title: "ExternalLink.AddExternalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalLink. Agrega un nombre externo"
type: docs
url: /es/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Agrega un nombre externo.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto del nombre externo. Si el nombre externo pertenece a una hoja de cálculo, el texto debe ser como Sheet1!Text. |
| referTo | String | El referTo del nombre externo. Debe ser una celda o el rango. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear un libro de trabajo externo de ejemplo
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Agregar enlace externo al libro de trabajo principal
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Agregar nombre externo
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Usar el nombre externo en una fórmula
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Calcular la fórmula
            workbook.CalculateFormula();
            
            // Mostrar el resultado
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


