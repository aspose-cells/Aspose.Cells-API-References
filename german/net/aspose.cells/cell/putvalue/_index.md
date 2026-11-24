---
title: "Cell.PutValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Fügt einen booleschen Wert in die Zelle ein"
type: docs
url: /de/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Schreibt einen booleschen Wert in die Zelle.

```csharp
public void PutValue(bool boolValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| boolValue | Boolean |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie einen booleschen Wert in Zelle B3 (Zeile 2, Spalte 2)
            cells[2, 2].PutValue(true);

            // Überprüfen Sie, ob der Wert korrekt gesetzt wurde
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Schreibt einen integer‑Wert in die Zelle.

```csharp
public void PutValue(int intValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| intValue | Int32 | Eingabewert |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Verwendung von PutValue mit Int32-Parametern
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Berechnen Sie die Summe der Werte
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Schreibt einen double‑Wert in die Zelle.

```csharp
public void PutValue(double doubleValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| doubleValue | Double | Eingabewert |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Setzen Sie Double-Werte mithilfe der PutValue-Methode
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Speichere die Arbeitsmappe
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Fügt einen Wert in die Zelle ein, bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | String | Eingabewert |
| isConverted | Boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | Boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zelle B3 abrufen
            Cell cell = worksheet.Cells["B3"];
            
            // Datenvalidierung für Alter festlegen (muss eine positive Zahl sein)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Wert einfügen mit Konvertierung und Validierungsprüfung
            cell.PutValue("-60", true, false);
            
            // Formeln berechnen (obwohl im einfachen Fall nicht nötig)
            workbook.CalculateFormula();
            
            // Überprüfen, ob der Wert gültig ist
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Arbeitsmappe speichern.
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Fügt einen Zeichenkettenwert in die Zelle ein und konvertiert den Wert bei Bedarf in einen anderen Datentyp.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | String | Eingabewert |
| isConverted | Boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Demonstriere PutValue mit String- und Booleschen Parametern
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Werte überprüfen
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Fügt einen Zeichenkettenwert in die Zelle ein.

```csharp
public void PutValue(string stringValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | String | Eingabewert |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Verwendung von PutValue mit String-Parametern
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Schreibt einen DateTime‑Wert in die Zelle.

```csharp
public void PutValue(DateTime dateTime)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dateTime | DateTime | Eingabewert |

### Hinweise

Das Festlegen eines DateTime-Werts für eine Zelle bedeutet nicht, dass die Zelle automatisch als Datum/Zeit formatiert wird. Der DateTime-Wert wird im Datenmodell von sowohl MS Excel als auch Aspose.Cells als numerischer Wert gespeichert. Ob der numerische Wert als solcher oder als Datum/Zeit interpretiert wird, hängt vom auf diese Zelle angewendeten Zahlenformat ab. Wenn diese Zelle nicht als Datum/Zeit formatiert ist, wird sie als numerischer Wert angezeigt, obwohl Sie ein DateTime eingegeben haben.

### Beispiele

Dieses Beispiel zeigt, wie man einen DateTime-Wert in einer Zelle setzt und ihn als Datum/Zeit anzeigen lässt.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Datum/Zeit in eine Zelle einfügen
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Schreibt einen Objektwert in die Zelle.

```csharp
public void PutValue(object objectValue)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objectValue | Object | Eingabewert |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue mit DateTime-Objekt
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue mit String-Objekt
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue mit numerischem Objekt
            cells[2, 0].PutValue((object)123.45);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


