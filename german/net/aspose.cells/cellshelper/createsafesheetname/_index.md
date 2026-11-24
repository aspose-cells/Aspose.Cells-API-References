---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Prüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette abgeschnitten, wenn die Länge das Limit überschreitet, und ungültige Zeichen werden durch   ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben."
type: docs
url: /de/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette gekürzt, falls die Länge das Limit überschreitet, und ungültige Zeichen werden durch ein Leerzeichen (' ') ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| nameProposal | String | zu verwendender Blattname |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen Namen. Wenn der angegebene Blattname den Regeln für Excel-Blattnamen entspricht, wird er zurückgegeben. Andernfalls wird die Zeichenkette gekürzt, falls die Länge das Limit überschreitet, und ungültige Zeichen werden durch das angegebene Zeichen ersetzt, dann wird der wiederhergestellte Zeichenkettenwert zurückgegeben.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| nameProposal | String | zu verwendender Blattname |
| replaceChar | Char | Zeichen, das verwendet wird, um ungültige Zeichen im angegebenen Blattnamen zu ersetzen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Beispiel 1: Sicheren Blattnamen mit Standard-Ersetzungszeichen erstellen
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Beispiel 2: Sicheren Blattnamen mit benutzerdefiniertem Ersetzungszeichen 'A' erstellen
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


