---
title: "Workbook.ImportXml"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Importa/Actualiza un archivo de datos XML en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Importa/Actualiza un archivo de datos XML en el libro de trabajo.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| url | String | la url/ruta del archivo xml. |
| sheetName | String | el nombre de la hoja de destino. |
| fila | Int32 | la fila de destino |
| col | Int32 | la columna de destino |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook wb = new Workbook();
            
            // Importar datos XML en la primera hoja de cálculo comenzando en la celda A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Importa/Actualiza un archivo de datos XML en el libro de trabajo.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | el flujo del archivo xml. |
| sheetName | String | el nombre de la hoja de destino. |
| fila | Int32 | la fila de destino. |
| col | Int32 | la columna de destino. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear datos XML de ejemplo
            string xmlData = @"<Products>
                <Product>
                    <Name>Laptop</Name>
                    <Price>999.99</Price>
                </Product>
                <Product>
                    <Name>Phone</Name>
                    <Price>699.99</Price>
                </Product>
            </Products>";

            // Convertir cadena XML a un MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Importar datos XML en el libro de trabajo comenzando en la celda A1 de la primera hoja de cálculo
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Guarda el libro de trabajo
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                xmlStream.Dispose();
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


