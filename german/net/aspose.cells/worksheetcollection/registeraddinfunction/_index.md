---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Fügt eine Add-In-Funktion in die Arbeitsmappe ein."
type: docs
url: /de/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Fügt die Add‑In‑Funktion in die Arbeitsmappe ein.

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| addInFile | String | die Datei enthält die Add‑In‑Funktionen |
| functionName | String | der Name der Add‑In‑Funktion |
| lib | Boolean | ob die angegebene Add‑In‑Datei im Verzeichnis oder Unterverzeichnis der Arbeitsbuch‑Add‑In‑Bibliothek liegt. Dieses Flag wird wirksam und macht einen Unterschied, wenn die angegebene addInFile ein relativer Pfad ist: true bedeutet, dass der Pfad relativ zur Add‑In‑Bibliothek ist, und false bedeutet, dass der Pfad relativ zu diesem Arbeitsbuch ist. |

### Rückgabewert

ID der Daten, die die angegebene Add‑In‑Funktion enthalten

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Hole das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispiel-Dateipfade festlegen (diese müssen in Ihrer Umgebung vorhanden sein)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Add‑In‑Funktionen mit unterschiedlichen Parametern registrieren
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Verwenden Sie die registrierten Funktionen in Zellen
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Speichere die Arbeitsmappe
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Fügt die Add‑In‑Funktion in die Arbeitsmappe ein.

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| id | Int32 | ID der Daten, die Add‑In‑Funktionen enthalten, kann durch den ersten Aufruf von `RegisterAddInFunction` für dieselbe Add‑In‑Datei erhalten werden. |
| functionName | String | der Name der Add‑In‑Funktion |

### Rückgabewert

URL der Add‑In‑Datei, die Add‑In‑Funktionen enthält

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erste Add‑In‑Funktion registrieren und deren ID erhalten
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Zweite Add‑In‑Funktion mit derselben ID registrieren
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Verwenden Sie die registrierten Funktionen in Formeln
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Speichere die Arbeitsmappe
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


