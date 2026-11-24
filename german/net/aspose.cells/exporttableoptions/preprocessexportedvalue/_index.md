---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Methode. Verarbeitet den Wert der aktuellen Zelle, die exportiert werden soll, vor"
type: docs
url: /de/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Verarbeitet den Wert der aktuellen zu exportierenden Zelle vor.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellRow | Int32 | der Zeilenindex der aktuellen Zelle |
| cellColumn | Int32 | der Spaltenindex der Zelle |
| Wert | CellValue | Wert und Typ der aktuellen Zelle |

### Rückgabewert

Ob die aktuelle Zelle durch einen anderen Typ und/oder Wert ersetzt wurde.

### Hinweise

Der Zeilen- und Spaltenindex ist der absolute Index der Zelle im Arbeitsblatt, nicht der Index in der exportierten Tabelle. Der Benutzer kann den Wert der aktuellen Zelle in der überschriebenen Implementierung dieser Methode prüfen; wenn die aktuelle Zelle durch einen anderen Typ und Wert ersetzt werden muss, sollte die Implementierung hier den erwarteten Typ und Wert im CellValue-Objekt setzen und true zurückgeben. Standardmäßig führt diese Methode nichts aus und gibt false zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten im Arbeitsblatt erstellen
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Erstelle eine Instanz von ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Erstelle ein CellValue-Objekt zur Demonstration
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Rufe PreprocessExportedValue mit spezifischen Parametern auf (Zeile 0, Spalte 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Zeige das Ergebnis des Methodenaufrufs an
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Modifiziere die Zelle bei Bedarf mit dem verarbeiteten Wert
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Speichere die Arbeitsmappe
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


