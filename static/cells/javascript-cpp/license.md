##License
Provides methods to license the component.
## License class
Provides methods to license the component.
### Example
In this example, an attempt will be made to find a license file named Aspose.Cells.lic in the input folder that contains the component, in the folder that contains the calling assembly,in the folder of the entry assembly and then in the embedded resources of the calling assembly.
```javascript
const { License } = AsposeCells;
var license = new License();
license.setLicense(data);
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of this class. |
## Methods
| Method | Description |
| --- | --- |
| [setLicense(string)](#setLicense-string-)| Licenses the component. |
| [setLicense(Uint8Array)](#setLicense-uint8array-)| Licenses the component. |
| static [encryptLicense(Uint8Array)](#encryptLicense-uint8array-)| Encrypts the license from Uint8Array. |
### constructor() {#constructor--}
Initializes a new instance of this class.
```javascript
constructor();
```
### setLicense(string) {#setLicense-string-}
Licenses the component.
```javascript
setLicense(licenseName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | string | The encrypted license file path. |
### setLicense(Uint8Array) {setLicense-uint8array-}
Licenses the component.
```javascript
setLicense(stream: Uint8Array): void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the encrypted license. |
### encryptLicense(Uint8Array) {encryptLicense-uint8array-}
Encrypts the license from Uint8Array.
```javascript
static encryptLicense(stream: Uint8Array): Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the license. |
**Returns**
A stream object contains the encrypted license.
