---
title: "Encoding Class"
linktitle: "Encoding"
articleTitle: "Encoding"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a character encoding."
type: docs
weight: 1940
url: /python-java/asposecells.api/encoding/
---

## Encoding class

Represents a character encoding.

## Methods

| Name | Description |
| --- | --- |
| [getASCII](#getascii) | Gets an encoding for the ASCII (7-bit) character set. |
| [getUTF7](#getutf7) | Gets an encoding for the UTF-7 format. |
| [getUTF8](#getutf8) | Gets an encoding for the UTF-8 format. |
| [getUTF8NoBOM](#getutf8nobom) | Gets an encoding for the UTF-8 format without the UTF-8 identifier. |
| [getUnicode](#getunicode) | Gets an encoding for the UTF-16 format using the little endian byte order. |
| [getBigEndianUnicode](#getbigendianunicode) | Gets an encoding for the UTF-16 format using the big endian byte order. |
| [getDefault](#getdefault) | Gets an encoding for the operating system's current ANSI code page. |
| [getEncoding](#getencoding) | Returns the encoding associated with the specified code page identifier. |
| [equals](#equals) | Determines whether the specified Object is equal to the current instance. |

### getASCII() {#getascii}

Gets an encoding for the ASCII (7-bit) character set.

**Returns:** A Encoding object for the ASCII (7-bit) character set.

### getUTF7() {#getutf7}

Gets an encoding for the UTF-7 format.

**Returns:** A Encoding object for the UTF-7 format.

### getUTF8() {#getutf8}

Gets an encoding for the UTF-8 format.

**Returns:** A Encoding object for the UTF-8 format.

### getUTF8NoBOM() {#getutf8nobom}

Gets an encoding for the UTF-8 format without the UTF-8 identifier.

**Returns:** A Encoding object for the UTF-8 format without UTF-8 identifier.

### getUnicode() {#getunicode}

Gets an encoding for the UTF-16 format using the little endian byte order.

**Returns:** A Encoding object for the UTF-16 format using the little endian byte

### getBigEndianUnicode() {#getbigendianunicode}

Gets an encoding for the UTF-16 format using the big endian byte order.

**Returns:** A Encoding object for the UTF-16 format using the big endian byte

### getDefault() {#getdefault}

Gets an encoding for the operating system's current ANSI code page.

**Returns:** An encoding for the operating system's current ANSI code page.

### getEncoding(codePage) (1 of 3) {#getencoding}

Returns the encoding associated with the specified code page identifier.

| Parameter | Type | Description |
| --- | --- | --- |
| codePage | int | The code page identifier of the preferred encoding. -or- 0, to use the default encoding. |

**Returns:** The Encoding object associated with the specified code page.

---

### getEncoding(charsetName) (2 of 3) {#getencoding-1}

Returns an encoding associated with the specified charset name.

| Parameter | Type | Description |
| --- | --- | --- |
| charsetName | String | specified charset name |

**Returns:** The Encoding object associated with the specified charset name.

---

### getEncoding(charset) (3 of 3) {#getencoding-2}

Returns an encoding associated with the specified charset object.

| Parameter | Type | Description |
| --- | --- | --- |
| charset | Charset | specified charset object |

**Returns:** The Encoding object associated with the specified charset object.

### equals(o) (1 of 2) {#equals}

Determines whether the specified Object is equal to the current instance.

| Parameter | Type | Description |
| --- | --- | --- |
| o | Object | The Object to compare with the current instance. |

**Returns:** true if value is an instance of Encoding and is equal to the current instance; otherwise, false.

---

### equals(other) (2 of 2) {#equals-1}

Determines whether the specified Encoding object is equal to the current instance.

| Parameter | Type | Description |
| --- | --- | --- |
| other | Encoding | The Encoding object to compare with the current instance. |

**Returns:** true if value is equal to the current instance; otherwise, false.
