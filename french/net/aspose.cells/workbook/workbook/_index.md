---
title: Workbook
second_title: Référence de l'API Aspose.Cells pour .NET
description: Initialise une nouvelle instance duWorkbookaspose.cells/workbook classe.
type: docs
weight: 10
url: /fr/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe.

```csharp
public Workbook()
```

### Remarques

Le type de format de fichier par défaut est Excel97To2003. Si vous souhaitez créer un autre type de fichier de format, veuillez appeler Workbook (FileFormatType fileFormatType).

### Exemples

Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe.

```csharp
[C#]

Workbook workbook = new Workbook();
		

[Visual Basic]

Dim workbook as Workbook = new Workbook()
		
```

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe.

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileFormatType | FileFormatType | Le nouveau format de fichier. |

### Remarques

Le type de format de fichier par défaut est Excel97To2003.

### Exemples

Le code suivant montre comment utiliser le constructeur Workbook pour créer et initialiser une nouvelle instance de la classe.

```csharp
[C#]

Workbook workbook = new Workbook(FileFormatType.Xlsx);
		

[Visual Basic]

Dim workbook as Workbook = new Workbook(FileFormatType.Xlsx)
		
```

### Voir également

* enum [FileFormatType](../../fileformattype)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_4}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe et ouvrez un fichier.

```csharp
public Workbook(string file)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| file | String | Le nom du fichier. |

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_2}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe et ouvrez un flux.

```csharp
public Workbook(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_5}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe et ouvrez un fichier.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| file | String | Le nom du fichier. |
| loadOptions | LoadOptions | Les options de charge |

### Voir également

* class [LoadOptions](../../loadoptions)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_3}

Initialise une nouvelle instance du[`Workbook`](../../workbook) classe et flux ouvert.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| loadOptions | LoadOptions | Les options de charge |

### Voir également

* class [LoadOptions](../../loadoptions)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
