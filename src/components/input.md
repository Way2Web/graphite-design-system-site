---
title: Components - gr-input
---

# gr-input

[[toc]]

Inputs can be used in forms, or anywhere where the user needs to provide information.

<gr-input></gr-input>

```html
<gr-input></gr-input>
```

## Examples

### Placeholders

Use the `placeholder` attribute to add a placeholder.

<gr-input placeholder="Type something"></gr-input>

```html
<gr-input placeholder="Type something"></gr-input>
```

### Clearable

Add the `clearable` attribute to add a clear button when the input has content.

<gr-input placeholder="Clearable" clearable></gr-input>

```html
<gr-input placeholder="Clearable" clearable></gr-input>
```

### Pill

Use the `pill` attribute to give inputs rounded edges.

<gr-input placeholder="Small" size="small" pill></gr-input>
<br>
<gr-input placeholder="Medium" size="medium" pill></gr-input>
<br>
<gr-input placeholder="Large" size="large" pill></gr-input>

```html
<gr-input placeholder="Small" size="small" pill></gr-input>
<br />
<gr-input placeholder="Medium" size="medium" pill></gr-input>
<br />
<gr-input placeholder="Large" size="large" pill></gr-input>
```

### Disabled

Use the `disabled` attribute to disable an input.

<gr-input placeholder="Disabled" size="small" disabled></gr-input>
<br>
<gr-input placeholder="Disabled" size="medium" disabled></gr-input>
<br>
<gr-input placeholder="Disabled" size="large" disabled></gr-input>

```html
<gr-input placeholder="Disabled" size="small" disabled></gr-input>
<br />
<gr-input placeholder="Disabled" size="medium" disabled></gr-input>
<br />
<gr-input placeholder="Disabled" size="large" disabled></gr-input>
```

### Sizes

Use the `size` attribute to change an input's size.

<gr-input placeholder="Small" size="small"></gr-input>
<br>
<gr-input placeholder="Medium" size="medium"></gr-input>
<br>
<gr-input placeholder="Large" size="large"></gr-input>

```html
<gr-input placeholder="Small" size="small"></gr-input>
<br />
<gr-input placeholder="Medium" size="medium"></gr-input>
<br />
<gr-input placeholder="Large" size="large"></gr-input>
```

### Invalid

The input can be marked invalid using the `invalid` attribute.

<gr-input placeholder="Invalid" invalid></gr-input>

```html
<gr-input placeholder="Invalid" invalid></gr-input>
```

### Labels

Use the `label` attribute to give the input an accessible label. For labels that contain HTML, use the `label` slot instead.

<gr-input label="What is your name?"></gr-input>

```html
<gr-input label="What is your name?"></gr-input>
```

### Help Text

Add descriptive help text to an input with the `help-text` attribute. For help texts that contain HTML, use the `help-text` slot instead.

<gr-input label="Nickname" help-text="What would you like people to call you?"></gr-input>

```html
<gr-input label="Nickname" help-text="What would you like people to call you?"></gr-input>
```

### Invalid Text

Add descriptive invalid text to an input with the `invalid-text` attribute. For invalid texts that contain HTML, use the `invalid-text` slot instead.

When you add the `invalid` attribute, the invalid text will be shown. When an input already includes help text, the help text is replaced with invalid text.

<gr-input label="Nickname" help-text="What would you like people to call you?" invalid-text="Enter what you would like people to call you." invalid></gr-input>

```html
<gr-input
  label="Nickname"
  help-text="What would you like people to call you?"
  invalid-text="Enter what you would like people to call you."
  invalid
></gr-input>
```

## Properties

| Property         | Attribute        | Description                                                                                                                                                                                               | Type       | Default          |
| ---------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------------- | -------- | ---------- | ---------- | ---------- | ------------------ | ------------ | ----------------- | ------------- | ------------------ | ---------- | ---------- | -------------- | ------------------ | --------------- | -------------------- | -------------- | ---------------- | --------------- | --------------- | --------------- | ---------------- | ---------------- | ---------------- | ---------------- | --------- | -------------- | ------------- | --------- | --------------- | -------------------- | ---------------- | ----------- | -------- | -------------- | ------------- | -------- | --------- | ---------------------- | -------------------- | ---------- | ------ | ---------- | ------------ | ----------- | ----- | ------------------ | -------------- | --------------- | ----------- | --------------- | ------ | -------- | ------- |
| `autocapitalize` | `autocapitalize` | Indicates whether and how the text value should be automatically capitalized as it is entered/edited by the user. Available options: `"off"`, `"none"`, `"on"`, `"sentences"`, `"words"`, `"characters"`. | `string`   | `'off'`          |
| `autocomplete`   | `autocomplete`   | Indicates whether the value of the control can be automatically completed by the browser.                                                                                                                 | `"email"   | "tel"            | "url"    | "off"      | "on"       | "name"     | "honorific-prefix" | "given-name" | "additional-name" | "family-name" | "honorific-suffix" | "nickname" | "username" | "new-password" | "current-password" | "one-time-code" | "organization-title" | "organization" | "street-address" | "address-line1" | "address-line2" | "address-line3" | "address-level4" | "address-level3" | "address-level2" | "address-level1" | "country" | "country-name" | "postal-code" | "cc-name" | "cc-given-name" | "cc-additional-name" | "cc-family-name" | "cc-number" | "cc-exp" | "cc-exp-month" | "cc-exp-year" | "cc-csc" | "cc-type" | "transaction-currency" | "transaction-amount" | "language" | "bday" | "bday-day" | "bday-month" | "bday-year" | "sex" | "tel-country-code" | "tel-national" | "tel-area-code" | "tel-local" | "tel-extension" | "impp" | "photo"` | `'off'` |
| `autocorrect`    | `autocorrect`    | Whether auto correction should be enabled when the user is entering/editing the text value.                                                                                                               | `"off"     | "on"`            | `'off'`  |
| `autofocus`      | `autofocus`      | This Boolean attribute lets you specify that a form control should have input focus when the page loads.                                                                                                  | `boolean`  | `false`          |
| `clearable`      | `clearable`      | Set to true to add a clear button when the input is populated.                                                                                                                                            | `boolean`  | `false`          |
| `debounce`       | `debounce`       | Set the amount of time, in milliseconds, to wait to trigger the `gr-change` event after each keystroke. This also impacts form bindings such as `ngModel` or `v-model`.                                   | `number`   | `0`              |
| `disabled`       | `disabled`       | Set to true to disable the input control.                                                                                                                                                                 | `boolean`  | `false`          |
| `enterkeyhint`   | `enterkeyhint`   | A hint to the browser for which enter key to display. Possible values: `"enter"`, `"done"`, `"go"`, `"next"`, `"previous"`, `"search"`, and `"send"`.                                                     | `"done"    | "enter"          | "go"     | "next"     | "previous" | "search"   | "send"`            | `undefined`  |
| `helpText`       | `help-text`      | The input's help text. Alternatively, you can use the help-text slot.                                                                                                                                     | `string`   | `''`             |
| `inputmode`      | `inputmode`      | The input's inputmode attribute.                                                                                                                                                                          | `"decimal" | "email"          | "none"   | "numeric"  | "search"   | "tel"      | "text"             | "url"`       | `undefined`       |
| `invalid`        | `invalid`        | Set to true to indicate this field is invalid. Will display the invalid text instead of the help text                                                                                                     | `boolean`  | `false`          |
| `invalidText`    | `invalid-text`   | The input's invalid text. Alternatively, you can use the invalid-text slot.                                                                                                                               | `string`   | `''`             |
| `label`          | `label`          | The inputs's label. Alternatively, you can use the label slot.                                                                                                                                            | `string`   | `''`             |
| `max`            | `max`            | The maximum value, which must not be less than its minimum (min attribute) value.                                                                                                                         | `string`   | `undefined`      |
| `min`            | `min`            | The minimum value, which must not be greater than its maximum (max attribute) value.                                                                                                                      | `string`   | `undefined`      |
| `name`           | `name`           | The input's name.                                                                                                                                                                                         | `string`   | `''`             |
| `pill`           | `pill`           | Set to true to draw a pill-style input with rounded edges.                                                                                                                                                | `boolean`  | `false`          |
| `placeholder`    | `placeholder`    | The input's placeholder text.                                                                                                                                                                             | `string`   | `''`             |
| `readonly`       | `readonly`       | If `true`, the user cannot modify the value.                                                                                                                                                              | `boolean`  | `false`          |
| `size`           | `size`           | The input's size.                                                                                                                                                                                         | `"large"   | "medium"         | "small"` | `'medium'` |
| `spellcheck`     | `spellcheck`     | If `true`, the element will have its spelling and grammar checked.                                                                                                                                        | `boolean`  | `false`          |
| `step`           | `step`           | Works with the min and max attributes to limit the increments at which a value can be set. Possible values are: `"any"` or a positive floating point number.                                              | `string`   | `undefined`      |
| `type`           | `type`           | The type of control to display. The default type is text.                                                                                                                                                 | `"date"    | "datetime-local" | "email"  | "month"    | "number"   | "password" | "search"           | "tel"        | "text"            | "time"        | "url"              | "week"`    | `'text'`   |
| `value`          | `value`          | The input's value attribute.                                                                                                                                                                              | `string`   | `''`             |

## Events

| Event       | Description                                 | Type                |
| ----------- | ------------------------------------------- | ------------------- |
| `gr-blur`   | Emitted when the control loses focus.       | `CustomEvent<void>` |
| `gr-change` | Emitted when the control's value changes.   | `CustomEvent<void>` |
| `gr-clear`  | Emitted when the clear button is activated. | `CustomEvent<void>` |
| `gr-focus`  | Emitted when the control gains focus.       | `CustomEvent<void>` |
| `gr-input`  | Emitted when the control receives input.    | `CustomEvent<void>` |

## Methods

### `removeFocus() => Promise<void>`

Removes focus from the input.

#### Returns

Type: `Promise<void>`

### `select() => Promise<void>`

Selects all the text in the input.

#### Returns

Type: `Promise<void>`

### `setFocus(options?: FocusOptions) => Promise<void>`

Sets focus on the input.

#### Returns

Type: `Promise<void>`

### `setRangeText(replacement: string, start: number, end: number, selectMode?: 'select' | 'start' | 'end' | 'preserve') => Promise<void>`

Replaces a range of text with a new string.

#### Returns

Type: `Promise<void>`

### `setSelectionRange(selectionStart: number, selectionEnd: number, selectionDirection?: 'forward' | 'backward' | 'none') => Promise<void>`

Sets the start and end positions of the text selection (0-based).

#### Returns

Type: `Promise<void>`

## Slots

| Slot             | Description                                                                                       |
| ---------------- | ------------------------------------------------------------------------------------------------- |
| `"help-text"`    | Help text that describes how to use the input.                                                    |
| `"invalid-text"` | Invalid text tells a user how to fix the error. Alternatively, you can use the invalid-text prop. |
| `"label"`        | The input's label. Alternatively, you can use the label prop.                                     |

## CSS Custom Properties

| Name                               | Description                                                                                  |
| ---------------------------------- | -------------------------------------------------------------------------------------------- |
| `--background-color`               | Background color of the input                                                                |
| `--background-color-focus`         | Background color of the input on focus                                                       |
| `--background-color-hover`         | Background color of the input on hover                                                       |
| `--background-color-invalid`       | Background color of the input when invalid                                                   |
| `--background-color-invalid-hover` | Background color of the input when invalid on focus                                          |
| `--border-color`                   | Border color of the input                                                                    |
| `--border-color-focus`             | Border color of the input on focus                                                           |
| `--border-color-hover`             | Border color of the input on hover                                                           |
| `--border-color-invalid`           | Border color of the input when invalid                                                       |
| `--border-color-invalid-hover`     | Border color of the input when invalid on focus                                              |
| `--border-radius`                  | Border radius of the input                                                                   |
| `--clear-icon-margin-end`          | Right margin of the clear icon (will be left margin when we support right-to-left direction) |
| `--color`                          | Text color of the input                                                                      |
| `--focus-ring`                     | The focus ring style to use when the input receives focus, a `box-shadow` property.          |
| `--font-size`                      | Font size of the input                                                                       |
| `--font-weight`                    | Font weight of the input                                                                     |
| `--min-height`                     | Minimum height of the input                                                                  |
| `--padding-end`                    | Right padding of the input (will be left padding when we support right-to-left direction)    |
| `--padding-start`                  | Left padding of the input (will be right padding when we support right-to-left direction)    |
| `--placeholder-color`              | Text color of the placeholder                                                                |
