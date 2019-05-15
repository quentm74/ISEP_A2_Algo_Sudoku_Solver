
# Sudoku solver

## Naming convention

> _example for a sudoku 9*9_

```
    0   1   2   3   4   5   6   7   8  
  ╔═══╤═══╤═══╦═══╤═══╤═══╦═══╤═══╤═══╗      ╔═══╤═══╤═══╗  
0 ║   │   │   ║   │   │   ║   │   │   ║      ║ 0 │ 1 │ 2 ║
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢      ╠───┼───┼───╢
1 ║  SQUARE0  ║  SQUARE1  ║  SQUARE2  ║      ║ 3 │ 4 │ 5 ║
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢      ╠───┼───┼───╢
2 ║   │   │   ║   │   │   ║   │   │   ║      ║ 6 │ 7 │ 8 ║
  ╠═══╪═══╪═══╬═══╪═══╪═══╬═══╪═══╪═══╣      ╚═══╩═══╩═══╝
3 ║   │   │   ║   │   │   ║   │   │   ║    Inside each square
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢    cells got an index
4 ║  SQUARE3  ║  SQUARE4  ║  SQUARE5  ║
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢
5 ║   │   │   ║   │   │   ║   │   │   ║
  ╠═══╪═══╪═══╬═══╪═══╪═══╬═══╪═══╪═══╣
6 ║   │   │   ║   │   │   ║   │   │   ║
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢
7 ║  SQUARE6  ║  SQUARE7  ║  SQUARE8  ║
  ╟───┼───┼───╫───┼───┼───╫───┼───┼───╢
8 ║   │   │   ║   │   │   ║   │   │   ║
  ╚═══╧═══╧═══╩═══╧═══╧═══╩═══╧═══╧═══╝
  <----------->
    square.lenght
  <----------------------------------->
    grid.size
```

If a cell must be empty, we put its value to 0.