---
title: "Workbook.GetFonts"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del libro de trabajo. Obtiene todas las fuentes en el pool de estilos"
type: docs
url: /es/net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

Obtiene todas las fuentes en el grupo de estilos.

```csharp
public Font[] GetFonts()
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetFontsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cree celdas con diferentes fuentes
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["A2"].PutValue("Sample Text 2");
            
            // Obtenga y modifique fuentes
            Font font1 = worksheet.Cells["A1"].GetStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            
            Font font2 = worksheet.Cells["A2"].GetStyle().Font;
            font2.Name = "Times New Roman";
            font2.Size = 14;
            font2.IsBold = true;

            // Obtener todas las fuentes usadas en el libro de trabajo
            Font[] fonts = workbook.GetFonts();
            Console.WriteLine("Total fonts in workbook: " + fonts.Length);
            
            // Mostrar información de la fuente
            foreach (Font font in fonts)
            {
                Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
            }
            
            // Guarde y vuelva a cargar para demostrar la persistencia
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Workbook loadedWorkbook = new Workbook(stream);
                Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
            }
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


