# Java Streams

A set of queries over a small in-memory employee dataset, each written as a single
stream pipeline. Java Lessons, task 7.

## What it covers

- `filter`, `map`, `sorted`, `reduce` and `collect` chained into one expression.
- Grouping and partitioning collectors for the department and salary breakdowns.
- Method references (`Employee::getName`) and comparator composition.
- `reduce` with `Double::sum` for aggregates such as the salary average.

Every query prints its number first, so the console output lines up with the task
sheet.

## Running it

```bash
javac -d out src/*.java
java -cp out Main
```

## Layout

- `src/Employee.java` - the model and the hard-coded dataset (`getData()`).
- `src/Department.java`, `src/Position.java` - the enums used for grouping.
- `src/Main.java` - the queries.
