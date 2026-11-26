---
title: "Workbook.Workbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor Workbook. Inicializa una nueva instancia de la clase Workbook"
type: docs
url: /es/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Inicializa una nueva instancia de la clase [`Workbook`](../).

```csharp
public Workbook()
```

### Observaciones

El tipo de formato de archivo predeterminado es Xlsx. Si desea crear otros tipos de archivos, utilice Workbook(FileFormatType).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo usando el constructor
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Guarda el libro de trabajo
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Inicializa una nueva instancia de la clase [`Workbook`](../).

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileFormatType | FileFormatType | El nuevo formato de archivo. |

### Observaciones

El tipo de formato de archivo predeterminado es Excel97To2003.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con formato de archivo XLSX
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poner algunos datos en la celda A1
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Inicializa una nueva instancia vacía de la clase [`Workbook`](../) con opciones

```csharp
public Workbook(LoadOptions loadOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadOptions | LoadOptions | Las opciones. |

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Inicializa una nueva instancia de la clase [`Workbook`](../) y abre un archivo.

```csharp
public Workbook(string file)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivo | String | El nombre del archivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // La ruta al directorio de documentos.
            string dataDir = "Your Document Directory";

            // Crear un Workbook a partir de un archivo Excel existente
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Mostrar alguna información de la hoja de cálculo
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Guardar el libro de trabajo en formato MHTML
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Crear otro Workbook a partir del archivo MHTML guardado
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Inicializa una nueva instancia de la clase [`Workbook`](../) y abre un flujo.

```csharp
public Workbook(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Crear un archivo Excel de muestra en memoria
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Crear una nueva instancia de Workbook usando el constructor Stream
                Workbook workbook = new Workbook(sampleStream);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];

                // Muestre los datos cargados
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Guardar el libro de trabajo en un archivo
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Inicializa una nueva instancia de la clase [`Workbook`](../) y abre un archivo.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| archivo | String | El nombre del archivo. |
| loadOptions | LoadOptions | Las opciones de carga |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga sin LightCellsDataHandler
            LoadOptions loadOptions = new LoadOptions();

            // Inicializar el libro de trabajo con la ruta del archivo y las opciones de carga
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Demostrar que el libro de trabajo está cargado accediendo al recuento de hojas de cálculo
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Inicializa una nueva instancia de la clase [`Workbook`](../) y abre un flujo.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo. |
| loadOptions | LoadOptions | Las opciones de carga |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un archivo Excel de muestra en memoria
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Crear LoadOptions con configuraciones específicas
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // Crear una instancia de Workbook usando el #ctor con Stream y LoadOptions
                Workbook workbook = new Workbook(stream, loadOptions);

                // Mostrar información básica sobre el libro de trabajo cargado
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Mostrar contenido de celda si está disponible
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Crear un archivo Excel simple en memoria para demostración
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Ver también

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


