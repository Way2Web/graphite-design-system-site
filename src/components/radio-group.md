---
title: Components - gr-radio-group
---

# gr-radio-group

[[toc]]

Radio Groups are used to group multiple radios so they function as a single control.

<gr-radio-group label="Select an item">
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>

```html
<gr-radio-group label="Select an item">
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>
```

## Examples

### Hiding the Fieldset

You can hide the fieldset and legend that wraps the radio group using the `no-fieldset` attribute. In this case, a label is still required for assistive devices to properly identify the control.

<gr-radio-group label="Select an item" no-fieldset>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>

```html
<gr-radio-group label="Select an item" no-fieldset>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>
```

### Invalid

The radio group can be marked invalid using the `invalid` attribute.

<gr-radio-group label="Select an item" invalid>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>
<br>
<gr-radio-group label="Select an item" no-fieldset invalid>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>

```html
<gr-radio-group label="Select an item" invalid>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>
<br />
<gr-radio-group label="Select an item" no-fieldset invalid>
  <gr-radio value="1" checked>Item 1</gr-radio>
  <gr-radio value="2">Item 2</gr-radio>
  <gr-radio value="3">Item 3</gr-radio>
</gr-radio-group>
```

## Properties

| Property              | Attribute               | Description                                                                                                   | Type      | Default        |
| --------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------- | --------- | -------------- |
| `allowEmptySelection` | `allow-empty-selection` | If `true`, the radios can be deselected.                                                                      | `boolean` | `false`        |
| `invalid`             | `invalid`               | Set to true to indicate this field is invalid.                                                                | `boolean` | `false`        |
| `label`               | `label`                 | The radio group label. Required for proper accessibility. Alternatively, you can use the label slot.          | `string`  | `''`           |
| `name`                | `name`                  | The name of the control, which is submitted with the form data.                                               | `string`  | `this.inputId` |
| `noFieldset`          | `no-fieldset`           | Hides the fieldset and legend that surrounds the radio group. The label will still be read by screen readers. | `boolean` | `false`        |
| `value`               | `value`                 | the value of the radio group.                                                                                 | `any`     | `undefined`    |

## Events

| Event       | Description                         | Type                                          |
| ----------- | ----------------------------------- | --------------------------------------------- |
| `gr-change` | Emitted when the value has changed. | `CustomEvent<WayRadioGroupChangeEventDetail>` |

## Slots

| Slot        | Description                                                                                          |
| ----------- | ---------------------------------------------------------------------------------------------------- |
| `(default)` | The default slot where radio controls are placed.                                                    |
| `"label"`   | The radio group label. Required for proper accessibility. Alternatively, you can use the label prop. |

## CSS Custom Properties

| Name                          | Description                                                                                  |
| ----------------------------- | -------------------------------------------------------------------------------------------- |
| `--border-color`              | Border color of the fieldset                                                                 |
| `--border-color-invalid`      | Border color of the fieldset when invalid                                                    |
| `--border-radius`             | Border radius of the fieldset                                                                |
| `--label-color`               | Color of the label                                                                           |
| `--label-padding-end`         | Right padding of the label (will be left padding when we support right-to-left direction)    |
| `--label-padding-start`       | Left padding of the label (will be right padding when we support right-to-left direction)    |
| `--margin-between-radios`     | Margin between the gr-radio children                                                         |
| `--padding-bottom`            | Bottom padding of the fieldset                                                               |
| `--padding-end`               | Right padding of the fieldset (will be left padding when we support right-to-left direction) |
| `--padding-start`             | Left padding of the fieldset (will be right padding when we support right-to-left direction) |
| `--padding-top`               | Top padding of the fieldset                                                                  |
| `--radio-label-color-invalid` | Color of the radio label's when invalid                                                      |
