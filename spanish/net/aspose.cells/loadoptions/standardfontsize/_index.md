---
title: "LoadOptions.StandardFontSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Establece el tamaño de fuente estándar predeterminado"
type: docs
url: /es/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Establece el tamaño de fuente estándar predeterminado.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // Cree opciones de carga HTML y establezca StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Acceder a la primera hoja de cálculo y a sus celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Establezca un texto de muestra y verifique las propiedades de la fuente
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


