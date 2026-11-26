---
title: "Workbook.Save"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Guarda el libro de trabajo en el disco"
type: docs
url: /es/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Guarda el libro de trabajo en el disco.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre del archivo. |
| saveFormat | SaveFormat | El tipo de formato de guardado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Guardar el libro de trabajo en formato XLSX
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Guardar el libro de trabajo en formato PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Guarda el libro de trabajo en el disco.

```csharp
public void Save(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Guardar el libro de trabajo en diferentes formatos usando un parámetro de cadena
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Guarda el libro de trabajo en el disco.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre del archivo. |
| saveOptions | SaveOptions | Las opciones de guardado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Crear opciones de guardado HTML y configurarlas
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Guardar el libro de trabajo con opciones
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Guarda el libro de trabajo en el flujo.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de archivo. |
| saveFormat | SaveFormat | El tipo de formato de archivo de guardado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo y agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Crear un flujo de memoria para guardar el libro de trabajo
                using (MemoryStream stream = new MemoryStream())
                {
                    // Guardar el libro de trabajo en el flujo en formato XLSX
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Mostrar mensaje de éxito
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // Restablecer la posición del flujo para un posible procesamiento adicional
                    stream.Position = 0;

                    // Opcionalmente guardar en un archivo para verificación
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Guarda el libro de trabajo en el flujo.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo de archivo. |
| saveOptions | SaveOptions | Las opciones de guardado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Crear un MemoryStream para guardar el libro de trabajo
            MemoryStream stream = new MemoryStream();

            try
            {
                // Crear SaveOptions para formato PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Guardar el libro de trabajo en el flujo con las opciones especificadas
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // Restablecer la posición del flujo para un posible uso posterior
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Crea la hoja de cálculo resultante y la transfiere al cliente, luego la abre en el navegador o en MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| respuesta | HttpResponse | Objeto de respuesta para devolver la hoja de cálculo al cliente. |
| fileName | String | El nombre del archivo creado. |
| contentDisposition | ContentDisposition | El tipo de disposición del contenido. |
| saveOptions | SaveOptions | Las opciones de guardado. |

### Observaciones

Este método está disponible solo para versiones net4.x.

### Ver también

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Crea la hoja de cálculo resultante y la transfiere al cliente, luego la abre en el navegador o en MS Workbook.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| respuesta | HttpResponse | Objeto de respuesta para devolver la hoja de cálculo al cliente. |
| fileName | String | El nombre del archivo creado. |
| contentDisposition | ContentDisposition | El tipo de disposición del contenido. |
| saveOptions | SaveOptions | Las opciones de guardado. |
| enableHttpCompression | Booleano | si se debe usar compresión http |

### Observaciones

Este método está disponible solo para versiones net4.x.

### Ver también

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


