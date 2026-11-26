---
title: "LoadOptions.StandardFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Establece el nombre de la fuente estándar predeterminada"
type: docs
url: /es/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Establece el nombre de la fuente estándar predeterminada

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice DefaultStyleSettings. Esta propiedad será eliminada 12 meses después desde marzo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Crear un archivo Excel de muestra en memoria
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Establecer opciones de carga con StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Cargar libro de trabajo con la fuente especificada
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Demostrar que la fuente está establecida comprobando el estilo predeterminado
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


