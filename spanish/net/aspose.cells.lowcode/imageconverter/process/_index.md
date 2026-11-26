---
title: "ImageConverter.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ImageConverter. Convierte el archivo de plantilla a imágenes"
type: docs
url: /es/net/aspose.cells.lowcode/imageconverter/process/
---
## Process(string, string) {#process_2}

Convierte el archivo de plantilla a imágenes.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| templateFile | String | El archivo de plantilla que se convertirá a imágenes. |
| resultFile | String | El archivo resultante (patrón de nombre) para las imágenes generadas. |

### Observaciones

Los archivos de salida se crearán a partir del archivo de resultado especificado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Image.png, los archivos de imagen generados serán Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y rellenarlo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Conversion Demo");
            worksheet.Cells["B3"].PutValue(DateTime.Now.ToString("yyyy-MM-dd"));

            // Guardar como archivo de plantilla para el procesamiento
            workbook.Save("Template.xlsx", SaveFormat.Xlsx);

            try
            {
                // Convertir la plantilla a imágenes usando parámetros (String, String)
                ImageConverter.Process("Template.xlsx", "OutputSheet.png");

                Console.WriteLine("Process method executed successfully. Generated image(s) from spreadsheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image conversion: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convierte el archivo de plantilla a imágenes

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones de salida y guardado |

### Observaciones

Al convertir a una imagen de formato que admite varias páginas (como tiff), el [`OutputFile`](../../lowcodesaveoptions/outputfile/) o [`OutputStream`](../../lowcodesaveoptions/outputstream/) especificado se utilizará directamente para la imagen resultante. Para otros tipos de imagen, si las opciones de guardado han especificado Stream como salida, entonces todas las imágenes resultantes se guardarán en el mismo Stream. De lo contrario, los archivos de salida se crearán a partir del archivo de salida especificado en las opciones de guardado añadiendo el número de secuencia de la hoja y la parte dividida. Por ejemplo, si el archivo de salida especificado es Image.png, los archivos de imagen generados serán Image_0_0.png, Image_0_1.png, ..., Image_1_0.png, ...

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            try
            {
                // Inicializar LowCodeLoadOptions con un archivo de plantilla
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions { InputFile = "template.xlsx" };
                
                // Inicializar LowCodeSaveOptions con el directorio de salida
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions { OutputFile = "output/" };
                
                // Ejecutar el método Process con los parámetros especificados
                ImageConverter.Process(loadOptions, saveOptions);
                
                Console.WriteLine("Spreadsheet converted to images successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during processing: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeSaveOptionsProvider) {#process_1}

Convierte el archivo de plantilla a imágenes

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeSaveOptionsProvider provider)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opciones de entrada y carga |
| saveOptions | LowCodeSaveOptions | Opciones para guardar. Su salida ([`OutputFile`](../../lowcodesaveoptions/outputfile/) o [`OutputStream`](../../lowcodesaveoptions/outputstream/)) no tiene efecto porque todas las salidas serán especificadas por el parámetro "provider". |
| provider | AbstractLowCodeSaveOptionsProvider | Proveedor de opciones de guardado para guardar las imágenes generadas |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class ImageConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
            const string templatePath = "SampleTemplate.xlsx";
            const string outputDir = "Output/";
            
            // Crear plantilla de ejemplo
            CreateTemplateFile(templatePath);
            Directory.CreateDirectory(outputDir);

            // Inicializar opciones de carga
            var loadOptions = new LowCodeLoadOptions()
            {
                InputFile = templatePath // Fixed property name
            };

            // Configurar opciones de guardado usando LowCodeImageSaveOptions
            var saveOptions = new LowCodeImageSaveOptions() // Corrected class
            {
                SaveFormat = SaveFormat.Png // Corrected property and enum
            };

            var provider = new DynamicSaveOptionsProvider(saveOptions);

            try
            {
                // Llamar al método estático Process
                ImageConverter.Process(loadOptions, saveOptions, provider);
                Console.WriteLine($"Generated PNG images in: {Path.GetFullPath(outputDir)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Processing failed: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string path)
        {
            using (Workbook wb = new Workbook())
            {
                Worksheet sheet = wb.Worksheets[0];
                sheet.Cells["A1"].PutValue("LowCode Process Demo");
                sheet.Cells["B3"].PutValue(DateTime.Now.ToString());
                wb.Save(path, SaveFormat.Xlsx);
            }
        }

        private class DynamicSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            private readonly LowCodeImageSaveOptions _baseOptions; // Corrected type

            public DynamicSaveOptionsProvider(LowCodeImageSaveOptions options)
            {
                _baseOptions = options;
            }

            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Acceder a las propiedades de resolución de LowCodeImageSaveOptions
                if (partInfo.SheetIndex == 0)
                {
                    _baseOptions.ImageOptions.HorizontalResolution = 300;
                    _baseOptions.ImageOptions.VerticalResolution = 300;
                }
                return _baseOptions;
            }
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [ImageConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


