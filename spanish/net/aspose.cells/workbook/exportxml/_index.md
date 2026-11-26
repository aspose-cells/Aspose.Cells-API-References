---
title: "Workbook.ExportXml"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Exporta datos XML vinculados mediante el mapa XML especificado"
type: docs
url: /es/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Exporta datos XML vinculados mediante el mapa XML especificado.

```csharp
public void ExportXml(string mapName, string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | String | nombre del mapa XML que necesita ser exportado |
| ruta | String | la ruta de exportación |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y cargar el archivo Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Obtener el primer XmlMap del libro de trabajo
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // Exportar datos XML usando el nombre del XmlMap y la ruta del archivo de salida
                wb.ExportXml(xmlMap.Name, "output.xml");
                Console.WriteLine("XML exported successfully to output.xml");
            }
            else
            {
                Console.WriteLine("No XmlMap found in the workbook");
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

## ExportXml(string, Stream) {#exportxml}

Exporta datos XML.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | String | nombre del mapa XML que necesita ser exportado |
| stream | Stream | el flujo de exportación |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y agregar algunos datos
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // Nombre del mapa XML a exportar – para propósitos de demostración usamos un nombre de marcador de posición
                string mapName = "SampleMap";

                try
                {
                    // Exportar el mapa XML a un archivo usando un FileStream (sobrecarga String, Stream)
                    string outputPath = "ExportedSample.xml";
                    using (FileStream fs = new FileStream(outputPath, FileMode.Create, FileAccess.Write))
                    {
                        workbook.ExportXml(mapName, fs);
                    }

                    Console.WriteLine($"ExportXml completed successfully. Output saved to '{outputPath}'.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during ExportXml: {ex.Message}");
                }
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


