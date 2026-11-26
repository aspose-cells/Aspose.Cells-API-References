---
title: "WorkbookSettings.ResourceProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo LinkToFile"
type: docs
url: /es/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Obtiene y establece el proveedor de flujo para recursos externos, como cargar datos de imagen para una imagen de tipo "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma de ejemplo para demostrar el proveedor de recursos
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Establecer el proveedor de recursos
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Guardar la forma como imagen usando el proveedor de recursos
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


