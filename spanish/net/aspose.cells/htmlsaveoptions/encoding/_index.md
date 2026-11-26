---
title: "HtmlSaveOptions.Encoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Si no se establece, use Encoding.UTF8 como tipo de codificación predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

Si no se establece, use Encoding.UTF8 como tipo de codificación predeterminado.

```csharp
public Encoding Encoding { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyEncodingDemo
    {
        private class SheetStreamProvider : IStreamProvider
        {
            private readonly MemoryStream _sheet1Stream;
            private readonly MemoryStream _sheet2Stream;
            private int _currentIndex = 0;

            public SheetStreamProvider(MemoryStream sheet1Stream, MemoryStream sheet2Stream)
            {
                _sheet1Stream = sheet1Stream;
                _sheet2Stream = sheet2Stream;
            }

            public void InitStream(StreamProviderOptions options)
            {
                // Inicialización si es necesario
            }

            public Stream GetStream(string sheetName)
            {
                return _currentIndex++ == 0 ? _sheet1Stream : _sheet2Stream;
            }

            public void CloseStream(StreamProviderOptions options)
            {
                options.Stream?.Flush();
            }
        }

        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a las hojas de cálculo
            workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
            workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer la codificación a UTF8
            saveOptions.Encoding = Encoding.UTF8;

            // Crear flujos de memoria para la salida
            using (MemoryStream sheet1Stream = new MemoryStream())
            using (MemoryStream sheet2Stream = new MemoryStream())
            {
                // Crear un proveedor de flujos para manejar múltiples hojas
                SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
                saveOptions.StreamProvider = streamProvider;

                // Guardar el libro de trabajo con opciones HTML
                workbook.Save(new MemoryStream(), saveOptions);

                // Verificar que el contenido se guardó con codificación UTF8
                string sheet1Content = Encoding.UTF8.GetString(sheet1Stream.ToArray());
                string sheet2Content = Encoding.UTF8.GetString(sheet2Stream.ToArray());

                Console.WriteLine("Sheet1 content contains text: " + 
                    sheet1Content.Contains("Sample content in Sheet1"));
                Console.WriteLine("Sheet2 content contains text: " + 
                    sheet2Content.Contains("Sample content in Sheet2"));
            }
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


