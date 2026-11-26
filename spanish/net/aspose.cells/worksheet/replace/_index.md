---
title: "Worksheet.Replace"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Reemplaza todo el texto de las celdas con una nueva cadena"
type: docs
url: /es/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

Reemplaza el texto de todas las celdas con una nueva cadena.

```csharp
public int Replace(string oldString, string newString)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldString | String | Valor de la cadena antigua. |
| newString | String | Valor de la cadena nueva. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // Agregar cuadro de texto con texto de ejemplo
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // Establecer encabezado y pie de página
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // Reemplazar "Hello" por "Hi" en todo el contenido
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // Reemplazar en encabezados/pies de página
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // Reemplazar en cuadros de texto
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


