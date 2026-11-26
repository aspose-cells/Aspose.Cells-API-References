---
title: "SheetSet.SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de SheetSet. Crea un conjunto de hojas basado en índices de hoja exactos"
type: docs
url: /es/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Crea un conjunto de hojas basado en índices de hoja exactos.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndexes | Int32[] | índices de hoja basados en cero. |

### Observaciones

Si se encuentra una hoja que no está en el libro de trabajo, se lanzará una excepción durante el renderizado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con 3 hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Agrega texto de identificación a cada hoja
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Crea SheetSet con índices de hoja específicos (0 y 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Crea opciones de guardado PDF con nuestro SheetSet
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Guarda el libro de trabajo con las hojas seleccionadas
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Crea un conjunto de hojas basado en nombres de hoja exactos.

```csharp
public SheetSet(params string[] sheetNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetNames | String[] | nombres de hoja. |

### Observaciones

Si se encuentra una hoja que no está en el libro de trabajo, se lanzará una excepción durante el renderizado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y agregar hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Preparar nombres de hoja para SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Crear SheetSet con parámetro de matriz de cadenas
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Configurar opciones de guardado PDF con el SheetSet creado
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Guardar el libro de trabajo en PDF con las hojas especificadas
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


