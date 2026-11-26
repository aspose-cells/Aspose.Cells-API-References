---
title: "WorkbookSettings.StreamProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el proveedor de flujo para recursos externos"
type: docs
url: /es/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Obtiene y establece el proveedor de flujo para recursos externos.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad ResourceProvider. Esta propiedad será eliminada 12 meses después desde junio de 2022. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Mostrar el valor actual de StreamProvider
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Establecer un proveedor de flujo personalizado
            settings.StreamProvider = new CustomStreamProvider1();

            // Agregar algunos datos para demostrar el uso del flujo
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Guardar el libro de trabajo - esto activará el proveedor de flujo
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Restablecer el proveedor de flujo
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Ver también

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


