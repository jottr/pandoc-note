Write notes in markdown and convert them to pdf via pandoc.  

```
$ task -- example.md 
```

## Table formatting

In Pandoc tables can be formatted in [multiple](https://pandoc.org/demo/example33/8.9-tables.html) ways.  

**Grid Tables** seem to be the most powerful variant with the least amount of formatting pitfalls.

**Example:**

```
+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+
```
