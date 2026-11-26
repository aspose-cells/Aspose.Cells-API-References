---
title: "DefaultStyleSettings.FontName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad DefaultStyleSettings. Obtiene/Establece el nombre de fuente predeterminado para el libro de trabajo"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Obtiene/Establece el nombre de fuente predeterminado para el libro de trabajo

```csharp
public string FontName { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crear opciones de carga y establecer el nombre de fuente
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Crear un nuevo libro de trabajo con las opciones de carga
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Acceder al estilo predeterminado y verificar el nombre de fuente
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Crear una hoja de cálculo y establecer el valor de la celda
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Guarda el libro de trabajo
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Ver también

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


