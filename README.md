# Get started

1. `npm install --save-dev flexy.grid`
2. `@import 'flexy';`
3. Head over to the [documentation](https://nguyenj.github.io/flexy/)
4. File [bugs and or issues](https://github.com/nguyenj/flexy/issues)

# Customizing

## Breakpoints

By default, the grid system is using a similar breakpoint label as Bootstrap: xs, sm, md, lg, xlg. However you can change these classes or limit the number of breakpoints to your needs. Instead of 5 different breakpoints, you can set 2 breakpoint with different labels. `$grid-settings` is a hash that you can override with your particular settings.

```
$grid-settings--animation: true !default;
$grid-settings--gutter: 1em !default;
$grid-settings--columns: 12 !default;
$grid-settings--offsets: true !default;
$grid-settings--breakpoints: (
  xs: 0,
  sm: 30em,
  md: 45em,
  lg: 60em
) !default;
$grid-settings--classes: (
  container: 'container',
  row: 'row',
  column: 'col',
  offset: 'offset'
) !default;
```

You can change the breakpoints like so:

```
$grid-settings--breakpoints: (
  mobile: 0,
  table: 48em
}
```

## Columns

The default grid system is generated with 12 columns; however, you're able to change the number of columns by changing the `$grid-settings.columns` to your needs:

```
$grid-settings--columns: 12;
```

## Column gutter

The default column gutter size is `1em`. The unit of the gutter does not have to be in `em`s, it could be in `px`s if that strikes your fancy.

You can change the width of the column gutter by changing `$grid-settings.gutter`:

```
$grid-settings--gutter: 1em;
```

## Animation

This isn't important; but if you like having the smooth transition in-between the breakpoints, you may turn this on:

```
$grid-settings--animation: true;
```
