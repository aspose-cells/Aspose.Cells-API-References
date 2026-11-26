---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se excluyen los estilos no utilizados. Para los archivos HTML generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita mantener todos los estilos en el libro para el HTML generado, como en el escenario en que el usuario necesita restaurar el libro desde el HTML generado más tarde, establezca esta propiedad como false."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Indica si se excluyen los estilos no utilizados. Para los archivos html generados, excluir los estilos no utilizados puede reducir el tamaño del archivo sin afectar los efectos visuales. Por lo tanto, el valor predeterminado de esta propiedad es true. Si el usuario necesita mantener todos los estilos en el libro de trabajo para el html generado (por ejemplo, si necesita restaurar el libro de trabajo a partir del html generado más tarde), establezca esta propiedad como false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra con diferentes estilos
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Configurar opciones de guardado HTML para excluir estilos no utilizados
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Guardar el libro de trabajo con opciones HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


