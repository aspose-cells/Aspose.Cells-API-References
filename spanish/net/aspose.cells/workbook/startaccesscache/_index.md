---
title: "Workbook.StartAccessCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Inicia la sesión que usa cachés para acceder a los datos"
type: docs
url: /es/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Inicia la sesión que usa cachés para acceder a los datos.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | AccessCacheOptions | opciones de acceso a datos |

### Observaciones

Si la caché del acceso a datos especificado requiere que algunos modelos de datos en la hoja de cálculo sean "solo lectura", entonces los modelos de datos correspondientes en cada hoja de cálculo de este libro de trabajo se considerarán "solo lectura" y el usuario no debe modificar ninguno de ellos. Después de terminar el acceso a los datos, [`CloseAccessCache`](../closeaccesscache/) debe invocarse con las mismas opciones para borrar todas las cachés y recuperar el modo de acceso normal.

### Ejemplos

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar formato condicional
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Establecer estilo para formato condicional
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Agregar algunas imágenes incrustadas
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Iniciar caché de acceso para un mejor rendimiento
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Acceder a los estilos de celda (será más rápido debido al almacenamiento en caché)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Cerrar la caché cuando haya terminado
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Ver también

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


