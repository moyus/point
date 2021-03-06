---
layout: master
title: Form
path:
  - Components
  - Form
catalogue:
  - Basic
  - Input
  - Select
  - Textarea
  - Range
  - Radio
  - Checkbox
  - Layout
---

# Form

Generic form controls.

## Basic

<section class="snippet">
  <div class="snippet__preview">
    <form>
      <div class="form-field">
        <label class="form-label">Email</label>
        <input type="email" class="form-input" placeholder="Enter Email" />
        <small class="form-help">Please provide a valid email address.</small>
      </div>
      <div class="form-field">
        <label class="form-label">Password</label>
        <input type="password" class="form-input" />
        <div class="form-help"></div>
      </div>
      <div class="form-field">
        <label class="flex items-center pointer">
          <input type="checkbox" class="form-checkbox" name="remember" id="remember">
          <span class="ml-3">Remember Me?</span>
        </label>
      </div>
      <div class="form-field">
        <button class="btn">Submit</button>
      </div>
    </form>
  </div>
  <div class="snippet__source">

```html
<form>
  <div class="form-field">
    <label class="form-label">Email</label>
    <input type="email" class="form-input" placeholder="Enter Email" />
    <small class="form-help">Please provide a valid email address.</small>
  </div>
  <div class="form-field">
    <label class="form-label">Password</label>
    <input type="password" class="form-input" />
    <div class="form-help"></div>
  </div>
  <div class="form-field">
    <label class="flex items-center pointer">
      <input type="checkbox" class="form-checkbox" name="remember" id="remember">
      <span class="ml-3">Remember Me?</span>
    </label>
  </div>
  <div class="form-field">
    <button class="btn">Submit</button>
  </div>
</form>
```

  </div>
</section>

## Input

The `.form-input` class is mean to be used on `<input>` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <input type="text" class="form-input" placeholder="Text input">
    </div>
    <div class="form-field">
      <input type="password" class="form-input" value="123456">
    </div>
    <div class="form-field">
      <input type="email" class="form-input" value="moyuboy@gmail.com">
    </div>
    <div class="form-field">
      <input type="url" class="form-input" value="https://github.com/moyus/point">
    </div>
    <div class="form-field">
      <input type="tel" class="form-input" value="010-123456">
    </div>
    <div class="form-field">
      <input type="number" class="form-input" value="666">
    </div>
    <div class="form-field">
      <input type="color" class="form-input">
    </div>
    <div class="form-field">
      <input type="date" class="form-input">
    </div>
    <div class="form-field">
      <input type="file" class="form-input">
    </div>
  </div>
  <div class="snippet__source">

```html
<input type="text" class="form-input" placeholder="Text input">
<input type="password" class="form-input" value="123456">
<input type="email" class="form-input" value="moyuboy@gmail.com">
<input type="url" class="form-input" value="https://github.com/moyus/point">
<input type="tel" class="form-input" value="010-123456">
<input type="number" class="form-input" value="666">
<input type="color" class="form-input">
<input type="date" class="form-input">
<input type="file" class="form-input">
```

  </div>
</section>

##### State

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <input type="text" class="form-input" placeholder="Normal state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input is-hovered" placeholder="Hovered state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input is-focused" placeholder="Focused state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input" readonly placeholder="Readonly state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input" disabled placeholder="Disabled state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input is-danger" placeholder="Negative state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input is-success" placeholder="Positive state">
    </div>
    <div class="form-field">
      <input type="text" class="form-input is-warning" placeholder="Warning state">
    </div>
  </div>
  <div class="snippet__source">

```html
<input type="text" class="form-input" placeholder="Normal state">
<input type="text" class="form-input is-hovered" placeholder="Hovered state">
<input type="text" class="form-input is-focused" placeholder="Focused state">
<input type="text" class="form-input" readonly placeholder="Readonly state">
<input type="text" class="form-input" disabled placeholder="Disabled state">
<input type="text" class="form-input is-danger" placeholder="Negative state">
<input type="text" class="form-input is-success" placeholder="Positive state">
<input type="text" class="form-input is-warning" placeholder="Warning state">
```

  </div>
</section>

##### Sizing

Your can create a small size of control by adding `.form-input--sm` or `.form-input--lg` modifier class on `.form-input` container.

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <input type="text" class="form-input form-input--sm" placeholder="Small sizing">
    </div>
    <div class="form-field">
      <input type="text" class="form-input" placeholder="Normal sizing">
    </div>
    <div class="form-field">
      <input type="text" class="form-input form-input--lg" placeholder="Large sizing">
    </div>
  </div>
  <div class="snippet__source">

```html
<input type="text" class="form-input form-input--sm" placeholder="Small sizing">
<input type="text" class="form-input" placeholder="Normal sizing">
<input type="text" class="form-input form-input--lg" placeholder="Large sizing">
```

  </div>
</section>

## Select

The `.form-select` class is mean to be used on `<select></select>` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label class="form-label">Single</label>
      <select class="form-select">
        <option value="0" selected>Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <label class="form-label">Multiple</label>
      <select class="form-select" multiple>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2" selected>Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
  </div>
  <div class="snippet__source">

```html
<div class="form-field">
  <label class="form-label">Single</label>
  <select class="form-select">
    <option value="0" selected>Beijing</option>
    <option value="1">Washington</option>
    <option value="2">Tokyo</option>
    <option value="3">London</option>
    <option value="4">Paris</option>
  </select>
</div>

<div class="form-field">
  <label class="form-label">Multiple</label>
  <select class="form-select" multiple>
    <option value="0">Beijing</option>
    <option value="1">Washington</option>
    <option value="2" selected>Tokyo</option>
    <option value="3">London</option>
    <option value="4">Paris</option>
  </select>
</div>
```

  </div>
</section>

##### State

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <select class="form-select">
        <option>Normal state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select is-hovered">
        <option>Hovered state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select is-focused">
        <option>Focused state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select" disabled>
        <option>Disabled state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select is-success">
        <option>Success state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select is-danger">
        <option>Danger state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select is-warning">
        <option>Warning state</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
  </div>
  <div class="snippet__source">

```html
<select class="form-select">...</select>
<select class="form-select is-hovered">...</select>
<select class="form-select is-focused">...</select>
<select class="form-select" disabled>...</select>
<select class="form-select is-success">...</select>
<select class="form-select is-danger">...</select>
<select class="form-select is-warning">...</select>
```

  </div>
</section>

##### Sizing

Your can create a small size of control by adding `.form-select--sm` or `.form-select--lg` modifier class on `.form-select` container.

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <select class="form-select form-select--sm">
        <option>Small sizing</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select">
        <option>Normal sizing</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
    <div class="form-field">
      <select class="form-select form-select--lg">
        <option>Large sizing</option>
        <option value="0">Beijing</option>
        <option value="1">Washington</option>
        <option value="2">Tokyo</option>
        <option value="3">London</option>
        <option value="4">Paris</option>
      </select>
    </div>
  </div>
  <div class="snippet__source">

```html
<select class="form-select form-select--sm">...</select>
<select class="form-select">...</select>
<select class="form-select form-select--lg">...</select>
```

  </div>
</section>

## Textarea

The `.form-textarea` class is mean to be used on `<textarea></textarea>` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <textarea class="form-textarea" rows="4"></textarea>
    </div>
  </div>
  <div class="snippet__source">

```html
<textarea class="form-textarea" rows="4"></textarea>
```

  </div>
</section>

##### State

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label class="form-label">Normal state</label>
      <textarea class="form-textarea" rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Hovered state</label>
      <textarea class="form-textarea is-hovered" rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Focused state</label>
      <textarea class="form-textarea is-focused" rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Readonly state</label>
      <textarea class="form-textarea" readonly rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Disabled state</label>
      <textarea class="form-textarea" disabled rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Success state</label>
      <textarea class="form-textarea is-success" rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Danger state</label>
      <textarea class="form-textarea is-danger" rows="2"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Warning state</label>
      <textarea class="form-textarea is-warning" rows="2"></textarea>
    </div>
  </div>
  <div class="snippet__source">

```html
<textarea class="form-textarea" rows="2"></textarea>
<textarea class="form-textarea is-hovered" rows="2"></textarea>
<textarea class="form-textarea is-focused" rows="2"></textarea>
<textarea class="form-textarea" readonly rows="2"></textarea>
<textarea class="form-textarea" disabled rows="2"></textarea>
<textarea class="form-textarea is-success" rows="2"></textarea>
<textarea class="form-textarea is-danger" rows="2"></textarea>
<textarea class="form-textarea is-warning" rows="2"></textarea>
```

  </div>
</section>

##### Sizing

Your can create a small size of control by adding `.form-textarea--sm` or `.form-textarea--lg` modifier class on `.form-textarea` container.

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label class="form-label">Small sizing</label>
      <textarea class="form-textarea form-textarea--sm" rows="4"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Normal sizing</label>
      <textarea class="form-textarea" rows="4"></textarea>
    </div>
    <div class="form-field">
      <label class="form-label">Large sizing</label>
      <textarea class="form-textarea form-textarea--lg" rows="4"></textarea>
    </div>
  </div>
  <div class="snippet__source">

```html
<textarea class="form-textarea form-textarea--sm" rows="4"></textarea>
<textarea class="form-textarea" rows="4"></textarea>
<textarea class="form-textarea form-textarea--lg" rows="4"></textarea>
```

  </div>
</section>

## Range

The `.form-range` class is mean to be used on `<input type="range">` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label for="gender" class="form-label">Quantity</label>
      <input type="range" name="quantity" class="form-range" min="1" max="100" step="1" value="10">
    </div>
  </div>
  <div class="snippet__source">

```html
<input type="range" name="quantity" class="form-range" min="1" max="100" step="1" value="10">
```

  </div>
</section>

## Radio

The `.form-radio` class is mean to be used on `<input type="radio">` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label for="gender" class="form-label">Gender</label>
      <div class="flex items-center">
        <label class="inline-flex items-center mr-5 pointer">
          <input type="radio" name="gender" class="form-radio" checked>
          <span class="ml-3">Male</span>
        </label>
        <label class="inline-flex items-center pointer">
          <input type="radio" name="gender" class="form-radio">
          <span class="ml-3">Female</span>
        </label>
      </div>
    </div>
  </div>
  <div class="snippet__source">

```html
<div class="form-field">
  <label for="gender" class="form-label">Gender</label>
  <div class="flex items-center">
    <label class="inline-flex items-center mr-5 pointer">
      <input type="radio" name="gender" class="form-radio">
      <span class="ml-3">Male</span>
    </label>
    <label class="inline-flex items-center pointer">
      <input type="radio" name="gender" class="form-radio">
      <span class="ml-3">Female</span>
    </label>
  </div>
</div>
```

  </div>
</section>

## Checkbox

The `.form-checkbox` class is mean to be used on `<input type="checkbox">` HTML element

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label class="flex items-center pointer">
        <input type="checkbox" class="form-checkbox" name="remember" id="remember">
        <span class="ml-3">Remember Me?</span>
      </label>
    </div>
  </div>
  <div class="snippet__source">

```html
<div class="form-field">
  <label class="flex items-center pointer">
    <input type="checkbox" class="form-checkbox" name="remember" id="remember">
    <span class="ml-3">Remember Me?</span>
  </label>
</div>
```

  </div>
</section>

## Layout

##### Field

Add structure to basic styled form controls

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <label class="form-label">Label text</label>
      <input type="text" class="form-input" placeholder="Form control">
      <small class="form-help">Some description text here...</small>
    </div>
  </div>
  <div class="snippet__source">

```html
<div class="form-field">
  <label class="form-label">Label text</label>
  <input type="text" class="form-input" placeholder="Form control">
  <small class="form-help">Some description text here...</small>
</div>
```

  </div>
</section>

##### Group

Group form controls on a single line

<section class="snippet">
  <div class="snippet__preview">
    <div class="form-field">
      <div class="form-group">
        <span class="form-addon">http://example.com/users/</span>
        <input type="text" class="form-input">
      </div>
    </div>
    <div class="form-field">
      <div class="form-group">
        <input type="text" class="form-input">
        <span class="form-addon">@example.com</span>
      </div>
    </div>
    <div class="form-field">
      <div class="form-group">
        <span class="form-addon">$</span>
        <input type="text" class="form-input">
        <span class="form-addon">.00</span>
      </div>
    </div>
    <div class="form-field">
      <div class="form-group">
        <span class="form-addon">From</span>
        <input type="date" class="form-input">
        <span class="form-addon">To</span>
        <input type="date" class="form-input">
      </div>
    </div>
    <div class="form-field">
      <div class="form-group">
        <span class="form-addon">
          <input type="radio" class="form-radio">
        </span>
        <input type="text" class="form-input">
      </div>
    </div>
    <div class="form-field">
      <div class="form-group">
        <input type="text" class="form-input">
        <span class="form-addon">
          <input type="checkbox" class="form-checkbox">
        </span>
      </div>
    </div>
  </div>
  <div class="snippet__source">

```html
<div class="form-field">
  <div class="form-group">
    <span class="form-addon">http://example.com/users/</span>
    <input type="text" class="form-input">
  </div>
</div>

<div class="form-field">
  <div class="form-group">
    <input type="text" class="form-input">
    <span class="form-addon">@example.com</span>
  </div>
</div>

<div class="form-field">
  <div class="form-group">
    <span class="form-addon">$</span>
    <input type="text" class="form-input">
    <span class="form-addon">.00</span>
  </div>
</div>

<div class="form-field">
  <div class="form-group">
    <span class="form-addon">From</span>
    <input type="date" class="form-input">
    <span class="form-addon">To</span>
    <input type="date" class="form-input">
  </div>
</div>

<div class="form-field">
  <div class="form-group">
    <span class="form-addon">
      <input type="radio" class="form-radio">
    </span>
    <input type="text" class="form-input">
  </div>
</div>

<div class="form-field">
  <div class="form-group">
    <input type="text" class="form-input">
    <span class="form-addon">
      <input type="checkbox" class="form-checkbox">
    </span>
  </div>
</div>
```

  </div>
</section>

##### Inline

Use flex utility classes to display a series of group elements on a single row

<section class="snippet">
  <div class="snippet__preview">
    <form class="inline-flex items-center">
      <input type="text" class="form-input">
      <button type="button" class="ml-3 btn btn--primary flex-no-shrink">Search</button>
    </form>
  </div>
  <div class="snippet__source">

```html
<form class="inline-flex items-center">
  <input type="text" class="form-input">
  <button type="button" class="ml-3 btn btn--primary flex-no-shrink">Search</button>
</form>
```

  </div>
</section>

##### Horizontal

Use Grid classes to create horizontal forms

<section class="snippet">
  <div class="snippet__preview">
    <form>
      <div class="row">
        <div class="col-3@md shown@md">
          <span class="form-label mt-3">Username</span>
        </div>
        <div class="col-9@md">
          <div class="form-field">
            <label class="form-label hidden@md">Username</label>
            <input type="text" class="form-input">
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-3@md shown@md">
          <span class="form-label mt-3">Password</span>
        </div>
        <div class="col-9@md">
          <div class="form-field">
            <label class="form-label hidden@md">Password</label>
            <input type="password" class="form-input">
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-9@md col-offset-3@md">
          <div class="form-field">
            <label class="inline-flex items-center pointer">
              <input type="checkbox" class="form-checkbox">
              <span class="ml-3">Remember me?</span>
            </label>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-9@md col-offset-3@md">
          <div class="form-field">
            <button type="button" class="btn btn--primary">Login</button>
          </div>
        </div>
      </div>
    </form>
  </div>
  <div class="snippet__source">

```html
<form>
  <div class="row">
    <div class="col-3@md shown@md">
      <span class="form-label mt-3">Username</span>
    </div>
    <div class="col-9@md">
      <div class="form-field">
        <label class="form-label hidden@md">Username</label>
        <input type="text" class="form-input">
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-3@md shown@md">
      <span class="form-label mt-3">Password</span>
    </div>
    <div class="col-9@md">
      <div class="form-field">
        <label class="form-label hidden@md">Password</label>
        <input type="password" class="form-input">
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-9@md col-offset-3@md">
      <div class="form-field">
        <label class="inline-flex items-center pointer">
          <input type="checkbox" class="form-checkbox">
          <span class="ml-3">Remember me?</span>
        </label>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-9@md col-offset-3@md">
      <div class="form-field">
        <button type="button" class="btn btn--primary">Login</button>
      </div>
    </div>
  </div>
</form>
```

  </div>
</section>
