---
title: Components - gr-checkbox
---

# gr-checkbox

[[toc]]

Checkboxes allow the user to toggle an option on or off.

<gr-checkbox>Checkbox</gr-checkbox>

```html
<gr-checkbox>Checkbox</gr-checkbox>
```

## Examples

### Checked

Use the `checked` attribute to activate the checkbox.

<gr-checkbox checked>Checked</gr-checkbox>

```html
<gr-checkbox checked>Checked</gr-checkbox>
```

### Indeterminate

Use the `indeterminate` attribute to make the checkbox indeterminate.

<gr-checkbox indeterminate>Indeterminate</gr-checkbox>

```html
<gr-checkbox indeterminate>Indeterminate</gr-checkbox>
```

### Disabled

Use the `disabled` attribute to disable the checkbox.

<gr-checkbox disabled>Disabled</gr-checkbox>

```html
<gr-checkbox disabled>Disabled</gr-checkbox>
```

### Invalid

The checkbox can be marked invalid using the `invalid` attribute.

<gr-checkbox invalid>Checkbox</gr-checkbox>

```html
<gr-checkbox invalid>Checkbox</gr-checkbox>
```

## Properties

| Property        | Attribute       | Description                                                     | Type      | Default        |
| --------------- | --------------- | --------------------------------------------------------------- | --------- | -------------- |
| `checked`       | `checked`       | Set to true to draw the checkbox in a checked state.            | `boolean` | `false`        |
| `disabled`      | `disabled`      | Set to true to disable the checkbox.                            | `boolean` | `false`        |
| `indeterminate` | `indeterminate` | Set to true to draw the checkbox in an indeterminate state.     | `boolean` | `false`        |
| `invalid`       | `invalid`       | Set to true to indicate this field is invalid.                  | `boolean` | `false`        |
| `name`          | `name`          | The name of the control, which is submitted with the form data. | `string`  | `this.inputId` |
| `value`         | `value`         | The checkbox's value attribute.                                 | `string`  | `undefined`    |

## Events

| Event       | Description                                       | Type                |
| ----------- | ------------------------------------------------- | ------------------- |
| `gr-blur`   | Emitted when the control loses focus.             | `CustomEvent<void>` |
| `gr-change` | Emitted when the control's checked state changes. | `CustomEvent<void>` |
| `gr-focus`  | Emitted when the control gains focus.             | `CustomEvent<void>` |

## Methods

### `removeFocus() => Promise<void>`

Removes focus from the checkbox.

#### Returns

Type: `Promise<void>`

### `setFocus(options?: FocusOptions) => Promise<void>`

Sets focus on the checkbox.

#### Returns

Type: `Promise<void>`

## Slots

| Slot        | Description           |
| ----------- | --------------------- |
| `(default)` | The checkboxes label. |

## CSS Custom Properties

| Name                                       | Description                                            |
| ------------------------------------------ | ------------------------------------------------------ |
| `--control-background-color`               | Background color of the control                        |
| `--control-background-color-checked`       | Background color of the control when checked           |
| `--control-background-color-checked-hover` | Background color of the control when checked on hover  |
| `--control-background-color-hover`         | Background color of the control on hover               |
| `--control-border-color`                   | Border color of the control                            |
| `--control-border-color-checked`           | Border color of the control when checked               |
| `--control-border-color-checked-hover`     | Border color of the control when checked on hover      |
| `--control-border-color-hover`             | Border color of the control on hover                   |
| `--control-color-checked`                  | Color of the control when checked (the checkmark icon) |
| `--control-size`                           | Size of the control                                    |
| `--label-color`                            | Color of the label                                     |
