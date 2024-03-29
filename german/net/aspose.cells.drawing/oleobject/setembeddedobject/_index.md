---
title: SetEmbeddedObject
second_title: Aspose.Cells für .NET-API-Referenz
description: Legt eingebettete Objektdaten fest.
type: docs
weight: 160
url: /de/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Legt eingebettete Objektdaten fest.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| linkToFile | Boolean | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn wahr, wird der Parameter objectData ignoriert. |
| objectData | Byte[] | Die eingebetteten Objektdaten. |
| sourceFileName | String | Der Dateiname. |
| displayAsIcon | Boolean | Gibt an, ob das Objekt als Symbol angezeigt wird. Wenn wahr, werden die ursprünglichen Bilddaten von Symbol verdeckt. |
| label | String | Das Symboletikett. Funktioniert nur, wenn displayAsIcon als wahr gilt. |

### Siehe auch

* class [OleObject](../../oleobject)
* namensraum [Aspose.Cells.Drawing](../../oleobject)
* Montage [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Legt eingebettete Objektdaten fest.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| linkToFile | Boolean | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn wahr, wird der Parameter objectData ignoriert. |
| objectData | Byte[] | Die eingebetteten Objektdaten. |
| sourceFileName | String | Der Dateiname. |
| displayAsIcon | Boolean | Gibt an, ob das Objekt als Symbol angezeigt wird. Wenn wahr, werden die ursprünglichen Bilddaten von Symbol verdeckt. |
| label | String | Das Symboletikett. Funktioniert nur, wenn displayAsIcon als wahr gilt. |
| updateIcon | Boolean | Gibt an, ob das Symbol automatisch aktualisiert wird. |

### Bemerkungen

Da Aspose alle Dateisymbole einbetten aktualisieren kann, ist es besser, wenn Sie das richtige Symbol mit hinzufügen können*updateIcon* als falsch.

### Siehe auch

* class [OleObject](../../oleobject)
* namensraum [Aspose.Cells.Drawing](../../oleobject)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
