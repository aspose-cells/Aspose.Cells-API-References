---
title: "Workbook.ImportXml"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Importa/Aggiorna un file di dati XML nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Importa/Aggiorna un file di dati XML nella cartella di lavoro.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| url | String | l'url/percorso del file xml. |
| sheetName | String | il nome del foglio di destinazione. |
| riga | Int32 | la riga di destinazione |
| col | Int32 | la colonna di destinazione |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook wb = new Workbook();
            
            // Importa i dati XML nel primo foglio di lavoro a partire dalla cella A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Importa/Aggiorna un file di dati XML nella cartella di lavoro.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | lo stream del file xml. |
| sheetName | String | il nome del foglio di destinazione. |
| riga | Int32 | la riga di destinazione. |
| col | Int32 | la colonna di destinazione. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea dati XML di esempio
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

            // Converti la stringa XML in un MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // Importa i dati XML nella cartella di lavoro a partire dalla cella A1 del primo foglio di lavoro
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Salva la cartella di lavoro
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Pulisci le risorse
                xmlStream.Dispose();
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


