# Zomboid-Map-Conflict-Checker

This is a simple tool to check for conflicts between mods that add new maps to Project Zomboid.

## Usage
First of all, you need to know the cells of the maps you want to check. Once you have them, you need a .csv file with the following format:

```csv
map1, cell1
map1, cell2; cell3; cell4
map2, cell5; cell6
map3, 38x38; 44x44; 50x50
```
The first column is the name of the map, and the second column is the cells that the map uses. To separate the 'names' column from the 'cells', you need to use a comma ( , ). To separate each cell, you need to use a semicolon ( ; ).

You can use spaces between the cells, but they are not necessary. The cells can be in any order, but they need to be in the same line and separated by semicolons NOT commas.

Do not put any special characters (quotes or double quotes e.g.) in the cells, only letters and numbers like this:

**GOOD:** 38x38; 44x44; 50x50 

**BAD:** '38x38', $44x44, '50X50', '62x62' 

The 'x' is not a special character, so you can use it in lower case only.

**EVERY CELL NEEDS TO BE ON THE FILE.**

If this example isnt clear enough, you can check the 'zomboid_maps'.csv file in this repository.

After that, you just need to add the .csv file with your maps to the same folder as the 'checker.exe' file and run it. **The file needs to be named "zomboid_maps.csv".**

Hope this helps!
If you have any questions or want to report a bug, you can contact me on Discord: [CocoDeLuta](https://discordapp.com/users/CocoDeLuta) or leave a bug report on the [Issues Page](https://github.com/CocoDeLuta/Zomboid-Map-Conflict-Checker/issues)
