# oui-formfield

<component-status cx-design="partial" ux="prototype"></component-status>

> **IMPORTANT:** The name of this component can still be changed at any moment.

oui-formfield is a package which provides styles for the formfield component.

## Installation

```less
@import 'oui-formfield/formfield';
```

## Usage

### Input

```html:preview
<div class="oui-input-formfield">
  <input type="text" id="text" name="text" class="oui-input" value="Input text" />
  <label for="text" class="oui-label">Label for Input</label>
</div>

<div class="oui-input-formfield">
  <input type="text-disabled" id="text-disabled" name="text-disabled" class="oui-input" value="Input text disabled" disabled />
  <label for="text-disabled" class="oui-label">Label for Input disabled</label>
</div>

<div class="oui-input-formfield">
  <input type="text-warning" id="text-warning" name="text-warning" class="oui-input oui-input_warning" value="Input text warning" />
  <label for="text-warning" class="oui-label">Label for Input warning</label>
</div>

<div class="oui-input-formfield">
  <input type="text-error" id="text-error" name="text-error" class="oui-input oui-input_error" value="Input text error" />
  <label for="text-error" class="oui-label">Label for Input error</label>
</div>

<div class="oui-input-group">
  <div class="oui-input-formfield">
    <input type="text" id="text-group" name="text-group" class="oui-input" value="Input text" />
    <label for="text-group" class="oui-label">Label for Input group</label>
  </div>
  <button class="oui-button">Go</button>
</div>
```

### Select

```html:preview
<div class="oui-select-formfield">
  <div class="oui-select">
    <select id="select" name="select" class="oui-select__input">
      <option value="Option 1">Option 1</option>
      <option value="Option 2">Option 2</option>
      <option value="Option 3">Option 3</option>
    </select>
    <i class="oui-icon oui-icon-chevron-down" aria-hidden="true"></i>
    <label for="select" class="oui-label">Label for Select</label>
  </div>
</div>

<div class="oui-select-formfield">
  <div class="oui-select">
    <select id="select-disabled" name="select-disabled" class="oui-select__input" disabled>
      <option value="Option 1">Option 1</option>
      <option value="Option 2">Option 2</option>
      <option value="Option 3">Option 3</option>
    </select>
    <i class="oui-icon oui-icon-chevron-down" aria-hidden="true"></i>
    <label for="select-disabled" class="oui-label">Label for Select disabled</label>
  </div>
</div>

<div class="oui-select-formfield">
  <div class="oui-select oui-select_warning">
    <select id="select-warning" name="select-warning" class="oui-select__input">
      <option value="Option 1">Option 1</option>
      <option value="Option 2">Option 2</option>
      <option value="Option 3">Option 3</option>
    </select>
    <i class="oui-icon oui-icon-chevron-down" aria-hidden="true"></i>
    <label for="select-warning" class="oui-label">Label for Select warning</label>
  </div>
</div>

<div class="oui-select-formfield">
  <div class="oui-select oui-select_error">
    <select id="select-error" name="select-error" class="oui-select__input">
      <option value="Option 1">Option 1</option>
      <option value="Option 2">Option 2</option>
      <option value="Option 3">Option 3</option>
    </select>
    <i class="oui-icon oui-icon-chevron-down" aria-hidden="true"></i>
    <label for="select-error" class="oui-label">Label for Select error</label>
  </div>
</div>
```

### Textarea

```html:preview
<div class="oui-textarea-formfield">
  <textarea class="oui-textarea" name="textarea-field" id="textarea-field">Textarea text</textarea>
  <label for="textarea-field" class="oui-label">Label for Textarea</label>
</div>

<div class="oui-textarea-formfield">
  <textarea class="oui-textarea" name="textarea-disabled" id="textarea-disabled" disabled>Textarea text disabled</textarea>
  <label for="textarea-disabled" class="oui-label">Label for Textarea disabled</label>
</div>

<div class="oui-textarea-formfield">
  <textarea class="oui-textarea oui-textarea_warning" name="textarea-warning" id="textarea-warning">Textarea text warning</textarea>
  <label for="textarea-warning" class="oui-label">Label for Textarea warning</label>
</div>

<div class="oui-textarea-formfield">
  <textarea class="oui-textarea oui-textarea_error" name="textarea-error" id="textarea-error">Textarea text error</textarea>
  <label for="textarea-error" class="oui-label">Label for Textarea error</label>
</div>
```

## Mixins

```less
@import 'oui-formfield/_mixins';
```

### .input-formfield

Define the base styles for an input group with label.

```less
#oui > .input-formfield();
```

```less
#oui > .input-formfield(
  @label-selector: Class,
  @input-selector: Class,
  @default-font-color: Color,
  @warning-font-color: Color,
  @error-font-color: Color,
  @font-weight: Number
);
```

### .select-formfield

Define the base styles for an select group with label.

```less
#oui > .select-formfield();
```

```less
#oui > .select-formfield(
  @label-selector: Class,
  @select-selector: Class,
  @default-font-color: Color,
  @warning-font-color: Color,
  @error-font-color: Color,
  @font-weight: Number
);
```

### .textarea-formfield

Define the base styles for an textarea group with label.
It inherits from `.input-formfield`.

```less
#oui > .textarea-formfield();
```

```less
#oui > .textarea-formfield(
  @label-selector: Class,
  @textarea-selector: Class,
  @default-font-color: Color,
  @warning-font-color: Color,
  @error-font-color: Color,
  @font-weight: Number
);
```
