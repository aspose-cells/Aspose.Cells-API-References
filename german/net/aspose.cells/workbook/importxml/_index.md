---
title: "Workbook.ImportXml"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Importiert/Aktualisiert eine XML-Datendatei in die Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

Importiert/aktualisiert eine XML‑Datendatei in die Arbeitsmappe.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| URL | String | die URL/der Pfad der XML-Datei. |
| sheetName | String | der Zielblattname. |
| row | Int32 | die Zielzeile |
| Spalte | Int32 | die Zielspalte |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook wb = new Workbook();
            
            // Importieren Sie XML-Daten in das erste Arbeitsblatt, beginnend bei Zelle A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

Importiert/aktualisiert eine XML‑Datendatei in die Arbeitsmappe.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | der XML-Datei-Stream. |
| sheetName | String | der Zielblattname. |
| row | Int32 | die Zielzeile. |
| Spalte | Int32 | die Zielspalte. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Beispieldaten im XML-Format erstellen
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

            // XML-Zeichenfolge in einen MemoryStream konvertieren
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // XML-Daten in die Arbeitsmappe importieren, beginnend bei Zelle A1 des ersten Arbeitsblatts
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // Speichere die Arbeitsmappe
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // Ressourcen bereinigen
                xmlStream.Dispose();
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


