# shell-data-processing

# Gitbash cheatsheet
```bash
curl "https://liftedlogic.com/3-examples-of-effective-homepage-design/?gclid=EAIaIQobChMIw_neprSw7gIVw_DACh2YFQApEAAYASAAEgLv4PD_BwE" -O "data.txt"
```
* Transform each space ' ' into a return character '\12'
```bash
 tr ' ' '\12' < data.txt
 ```
 * Pipe the output to sort 
 ```bash
 tr ' ' '\12' < data.txt | sort
 ```
 * Pipe the sorted output to uniq -c to count
 ```bash
 tr ' ' '\12' < data.txt | sort | uniq -c
 ```
 * Pipe the reduced output to sort with -nr flag
 ```bash
 tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr
 ```
 * output to result.txt
 ```bash
 tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt
 ```
 [data.txt]! (https://github.com/Ravichanderreddy-goli/shell-data-processing/blob/master/data.txt)
 [results.txt]! (https://github.com/Ravichanderreddy-goli/shell-data-processing/blob/master/result.txt)
