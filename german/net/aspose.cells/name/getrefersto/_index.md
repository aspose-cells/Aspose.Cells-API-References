---
title: "Name.GetRefersTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Methode. Ruft die Referenz dieses Namens ab"
type: docs
url: /de/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Lese die Referenz dieses Namens.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Referenz im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Referenz nach den Ländereinstellungen formatiert werden muss. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Rufen Sie GetRefersTo mit R1C1-Format und lokalem Geltungsbereich auf
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // Rufen Sie GetRefersTo mit A1-Format und globalem Geltungsbereich auf
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Details des benannten Bereichs anzeigen
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Lese die Referenz dieses Namens basierend auf der angegebenen Zelle.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Referenz im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Referenz nach den Ländereinstellungen formatiert werden muss. |
| row | Int32 | Der Zeilenindex der Zelle. |
| column | Int32 | Der Spaltenindex der Zelle. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Rufen Sie GetRefersTo mit spezifischen Parametern (isR1C1, isLocal, row, column) auf
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Den benannten Bereich basierend auf dem Ergebnis ändern
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


