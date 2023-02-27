---
sidebar_position: 10
---

# Tables

The look of an HTML table can be greatly improved with CSS:

| Company                      | Contact            | Country |
| ---------------------------- | ------------------ | ------- |
| Alfreds Futterkiste          | Maria Anders       | Germany |
| Berglunds snabbköp           | Christina Berglund | Sweden  |
| Centro comercial Moctezuma   | Francisco Chang    | Mexico  |
| Ernst Handel                 | Roland Mendel      | Austria |
| Island Trading               | Helen Bennett      | UK      |
| Königlich Essen              | Philip Cramer      | Germany |
| Laughing Bacchus Winecellars | Yoshi Tannamuri    | Canada  |
| Magazzini Alimentari Riuniti | Giovanni Rovelli   | Italy   |

## Table Borders

To specify table borders in CSS, use the border property.

The example below specifies a solid border for `<table>`, `<th>`, and `<td>` elements:

| Firstname | Lastname |
| --------- | -------- |
| Peter     | Griffin  |
| Lois      | Griffin  |

```css
table,
th,
td {
  border: 1px solid;
}
```

## Full-Width Table

The table above might seem small in some cases. If you need a table that should span the entire screen (full-width), add width: 100% to the `<table>` element:

```css
table {
  width: 100%;
}
```

:::

Notice that the table in the examples above have double borders. This is because both the table and the `<th>` and `<td>` elements have separate borders.

To remove double borders, take a look at the example below.
:::

## Collapse Table Borders

The `border-collapse` property sets whether the table borders should be collapsed into a single border:

```css
table {
  border-collapse: collapse;
}
```

If you only want a border around the table, only specify the `border` property for `<table>`:

```css
table {
  border: 1px solid;
}
```
