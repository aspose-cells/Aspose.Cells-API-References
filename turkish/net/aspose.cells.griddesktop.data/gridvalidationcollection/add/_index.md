---
title: "GridValidationCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridValidationCollection yöntemi. Bir GridValidation öğesini koleksiyona ekler. Doğrulama belirtilen hücreye uygulanır."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Koleksiyona bir [`GridValidation`](../../gridvalidation/) ekleyin. Doğrulama belirtilen hücreye uygulanır.

```csharp
public GridValidation Add(string cellname)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellname | String | hücrenin adı. |

### Dönüş Değeri

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Ayrıca Bakınız

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Koleksiyona bir [`GridValidation`](../../gridvalidation/) ekleyin. Doğrulama belirtilen hücreye uygulanır.

```csharp
public GridValidation Add(int row, int col)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satır indeksi. |
| col | Int32 | Hücrenin sütun indeksi. |

### Dönüş Değeri

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Ayrıca Bakınız

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Belirtilen hücreye hücre adıyla bir doğrulama ekler.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Izgara hücresinin adı. |
| isRequired | Boolean | Hücre değerinin gerekli olup olmadığını gösteren değer. |
| regEx | String | Düzenli ifade. |

### Ayrıca Bakınız

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Satır ve sütun indeksinde belirtilen hücreye bir doğrulama ekler.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satır indeksi. |
| col | Int32 | Hücrenin sütun indeksi. |
| customValidation | ICustomValidation | Özel doğrulama nesnesi. |

### Ayrıca Bakınız

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Satır ve sütun indeksinde belirtilen hücreye bir doğrulama ekler.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satır indeksi. |
| col | Int32 | Hücrenin sütun indeksi. |
| isRequired | Boolean | Hücre değerinin gerekli olup olmadığını gösteren değer. |
| regEx | String | Düzenli ifade. |

### Ayrıca Bakınız

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Belirtilen hücreye hücre adıyla bir doğrulama ekler.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Izgara hücresinin adı. |
| customValidation | ICustomValidation | Özel doğrulama nesnesi. |

### Ayrıca Bakınız

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


