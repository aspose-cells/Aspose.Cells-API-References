---
title: "Cell.SetTableFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Erstelle eine zweivariable Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle"
type: docs
url: /de/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| rowInputCell | String | die Zeileneingabezelle |
| columnInputCell | String | die Spalteneingabezelle |
| Werte | Object[][] | Werte für Zellen im Tabellenformelbereich |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Zielzelle, in der die Tabellenformel festgelegt wird
            Cell targetCell = worksheet.Cells["C3"];

            // Parameter für SetTableFormula vorbereiten
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Tabellenformel in der Zielzelle festlegen
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Arbeitsmappen-Formeln berechnen, um Ergebnisse zu aktualisieren
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| Eingabezelle | String | die Eingabezelle |
| isRowInput | Boolean | Gibt an, ob die Eingabezelle eine Zeileneingabezelle (true) oder eine Spalteneingabezelle (false) ist. |
| Werte | Object[][] | Werte für Zellen im Tabellenformelbereich |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Parameter für SetTableFormula vorbereiten
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Zielzelle für Datentabelle abrufen (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Rufen Sie SetTableFormula mit Zinsvariationen auf
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Formeln berechnen, um Tabellenergebnisse zu aktualisieren
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Erstellt eine zweidimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| rowIndexOfRowInputCell | Int32 | Zeilenindex der Zeileneingabezelle |
| columnIndexOfRowInputCell | Int32 | Spaltenindex der Zeileneingabezelle |
| rowIndexOfColumnInputCell | Int32 | Zeilenindex der Spalteneingabezelle |
| columnIndexOfColumnInputCell | Int32 | Spaltenindex der Spalteneingabezelle |
| Werte | Object[][] | Werte für Zellen im Tabellenformelbereich |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Eingabewerte für Datentabelle vorbereiten (Zinssätze und Darlehensbeträge)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Tabellenformel setzen mit 3x3-Datentabelle-Dimensionen und Eingabezellen-Offsets
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Erstellt eine eindimensionale Datentabelle für den angegebenen Bereich, beginnend mit dieser Zelle.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNumber | Int32 | Anzahl der Zeilen, die mit der Formel befüllt werden sollen. |
| columnNumber | Int32 | Anzahl der Spalten, die mit der Formel befüllt werden sollen. |
| rowIndexOfInputCell | Int32 | Zeilenindex der Eingabezelle |
| columnIndexOfInputCell | Int32 | Spaltenindex der Eingabezelle |
| isRowInput | Boolean | Gibt an, ob die Eingabezelle eine Zeileneingabezelle (true) oder eine Spalteneingabezelle (false) ist. |
| Werte | Object[][] | Werte für Zellen im Tabellenformelbereich |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Beispiel-Datenarray für Tabellenformel-Parameter erstellen
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Zielzelle abrufen, um Tabellenformel anzuwenden
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Tabellenformel setzen mit: 
                // 3 Zeilen, 2 Spalten, Eingabezelle bei A1 (0,0), 
                // Zeileneingabetyp und Beispielwerte
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


