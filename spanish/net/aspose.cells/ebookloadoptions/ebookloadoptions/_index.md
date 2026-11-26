---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de EbookLoadOptions. Crea una opción para cargar el archivo ebook"
type: docs
url: /es/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Crea una opción para cargar el archivo ebook.

```csharp
public EbookLoadOptions()
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Cree una instancia de EbookLoadOptions usando el constructor
            EbookLoadOptions options = new EbookLoadOptions();

            // Establecer algunas propiedades básicas
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Cargue un archivo ebook con las opciones especificadas
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Guardar como archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Crea una opción de carga del archivo ebook.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de carga |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Cree una instancia de EbookLoadOptions con el parámetro LoadFormat
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Mostrar confirmación
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Ejemplo de uso: Cargue un libro de trabajo con estas opciones
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Guardar el resultado
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


