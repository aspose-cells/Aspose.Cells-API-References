---
title: "IExportObjectListener.ExportObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IExportObjectListener. Exporta un objeto"
type: docs
url: /es/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Exporta un objeto.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| e | ExportObjectEvent | El evento que se dispara cuando un objeto necesita ser exportado. |

### Valor de retorno

La información sobre el resultado de la exportación del objeto. Al exportar objetos cuando se exporta el libro de trabajo al formato HTML, el resultado es una cadena URL para acceder a la Imagen guardada del archivo html que contiene este objeto exportado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Crear una instancia de la clase de demostración que implementa IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // En un escenario real, el ExportObjectEvent sería proporcionado por el framework
                // Para propósitos de demostración, simplemente llamaremos al método con null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Implementación personalizada para manejar la exportación
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Devuelve un objeto modificado o null para usar el comportamiento de exportación predeterminado
            return null;
        }
    }
}
```

### Ver también

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


