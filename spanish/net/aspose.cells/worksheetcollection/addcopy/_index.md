---
title: "WorksheetCollection.AddCopy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Añade una hoja de cálculo a la colección y copia datos de una hoja existente"
type: docs
url: /es/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

```csharp
public int AddCopy(string sheetName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | String | Nombre de la hoja de cálculo origen. |

### Valor de retorno

[`Worksheet`](../../worksheet/) object index.

### Excepciones

| excepción | condición |
| --- | --- |
| [CellsException](../../cellsexception/) | Especifica un nombre de hoja de cálculo no válido. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo llamada "Original" al libro
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Agregar algunos datos a la hoja original
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Crear una copia de la hoja "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Modificar la hoja copiada para demostrar que es una copia independiente
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente.

```csharp
public int AddCopy(int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | Índice de la hoja de cálculo origen. |

### Valor de retorno

[`Worksheet`](../../worksheet/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y agregar algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Agregar una copia de la primera hoja de cálculo
            workbook.Worksheets.AddCopy(0);
            
            // Verificar que se creó la copia
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copiar un grupo de hojas de cálculo.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Worksheet[] | Las hojas de cálculo origen. |
| destSheetNames | String[] | Los nombres de las hojas copiadas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo de ejemplo
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Poblar algunos datos en las hojas de cálculo
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Preparar la matriz de hojas de cálculo de origen
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Preparar la matriz de nombres de hojas de destino
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Llamar al método AddCopy con los parámetros (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Verificar que se crearon las copias
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


