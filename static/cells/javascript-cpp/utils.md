##Utils
Provides utility functions for loading font data, ICU data, and exception message handling.
## Utils class
Provides utility functions for loading font data, ICU data, and exception message handling.
## Methods
| Method | Description |
| --- | --- |
| static [loadICUData(string)](#loadICUData-string-)| Loads ICU data from a local file path. |
| static [loadICUData(Uint8Array)](#loadICUData-uint8array-)| Loads ICU data from Uint8Array. |
| static [loadFont(Uint8Array)](#loadFont-uint8array-)| Loads font data from Uint8Array. |
| static [fetchWasmError(number)](#fetchWasmError-number-)| Fetches the error message from WebAssembly by the exception address. |
### loadICUData(string) {#loadICUData-string-}
Loads ICU data from a local file path.
```javascript
static loadICUData(dataFilePath: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataFilePath | string | The ICU data file path. |
### loadICUData(Uint8Array) {loadICUData-uint8array-}
Loads ICU data from Uint8Array.
```javascript
static loadICUData(stream: Uint8Array): void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the ICU data. |
### loadFont(Uint8Array) {loadFont-uint8array-}
Loads font data from Uint8Array.
```javascript
static loadFont(stream: Uint8Array): void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the font data. |
### fetchWasmError(number) {fetchWasmError-number-}
Fetches the error message from WebAssembly by the exception address.
```javascript
static fetchWasmError(err: number): string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| err | number | The exception address in WebAssembly. |
