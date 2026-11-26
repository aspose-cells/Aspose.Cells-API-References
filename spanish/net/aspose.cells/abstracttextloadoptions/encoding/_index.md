---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractTextLoadOptions. Obtiene y establece la codificación predeterminada. Solo se aplica a archivos csv"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Obtiene y establece la codificación predeterminada. Solo se aplica a archivos csv.

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
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crear datos CSV de ejemplo con codificación ASCII
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // Cargar el libro de trabajo con la codificación ASCII especificada
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Mostrar los datos cargados
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Agregar texto Unicode
            cells[2, 0].PutValue("日本語のテキスト");
            
            // Guardar con codificación UTF-8
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // Mostrar los primeros bytes para mostrar el BOM UTF-8
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Ver también

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


