---
title: "OdsPageBackground.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece el tipo de fondo de página"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Obtiene y establece el tipo de fondo de página.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la configuración de página de la primera hoja de cálculo
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Obtenga el fondo de página ODS
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Establezca el tipo de fondo a gráfico y configúrelo
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Guarda el libro de trabajo
            workbook.Save("output.ods");
            
            // Recargue el archivo guardado para verificar la configuración
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Salida de los resultados de verificación
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Ver también

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


