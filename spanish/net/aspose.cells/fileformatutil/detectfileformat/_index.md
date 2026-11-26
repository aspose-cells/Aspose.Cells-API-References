---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Detecta y devuelve la información sobre el formato de un Excel almacenado en un stream"
type: docs
url: /es/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream |  |

### Valor de retorno

Un objeto [`FileFormatInfo`](../../fileformatinfo/) que contiene la información detectada.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Preparar un MemoryStream con los datos del libro de trabajo
            using (MemoryStream stream = new MemoryStream())
            {
                // Guardar el libro de trabajo en el flujo en formato XLSX
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Detectar el formato de archivo desde el flujo
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Mostrar los resultados de detección
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Guardar el libro de trabajo original para verificación
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream |  |
| contraseña | String | La contraseña para archivos ooxml encriptados. |

### Valor de retorno

Un objeto [`FileFormatInfo`](../../fileformatinfo/) que contiene la información detectada.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            
            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
                Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
            }

            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
            }
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Detecta y devuelve la información sobre un formato de un Excel almacenado en un archivo.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |

### Valor de retorno

Un objeto [`FileFormatInfo`](../../fileformatinfo/) que contiene la información detectada.

### Observaciones

Solo admite la comprobación de algunos archivos con firma mágica. Si no hay firma mágica, no podemos detectar con precisión el formato del archivo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            
            Console.WriteLine("Load Format: " + info.LoadFormat);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
            
            Console.WriteLine("Save Format: " + saveFormat);
            Console.WriteLine("Load Format (converted): " + loadFormat);
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Detecta y devuelve la información sobre un formato de un Excel almacenado en un archivo.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | String | La ruta del archivo. |
| contraseña | String | La contraseña para archivos ooxml encriptados. |

### Valor de retorno

Un objeto [`FileFormatInfo`](../../fileformatinfo/) que contiene la información detectada.

### Observaciones

Solo admite la comprobación de algunos archivos con firma mágica. Si no hay firma mágica, no podemos detectar con precisión el formato del archivo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
    {
        public static void Run()
        {
            string sourcePath = @"..\..\..\Data\";
            
            // Detectar formato de archivo XLSX
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // Detectar formato de archivo DOCX
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


