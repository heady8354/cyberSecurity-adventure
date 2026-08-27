today was a much needed success. small and short, only about an hour long, but i learned a lot. command line arguments, and running python scripts off them. 

so basically, python has something you can import, `sys`. importing sys allows you to check each parameter of a command line. so you do, say: `python script.py`. if you do print(sys.argv[0]), you get `script.txt`. pretty cool! so, with this information, i made a short script which looks for every instance of a keyword on every line of a file. here it is:

```python 
import sys
print(sys.argv[0] + " is the script name")
print(sys.argv[1] + " is the file you're looking inside of")
print(sys.argv[2] + " is the word you're looking for")
with open(sys.argv[1]) as f: # f = file
    line = 0
    for x in f: # x = line (for line in file)
        line = line + 1
        if sys.argv[2] in x:
            print("found " + str(sys.argv[2]) + " on line " + str(line) + "!")
```

primitive, yes, but i sure as hell couldnt do this 3 days ago. 
its late, so i shall call it here. good progress, but not enough for a job. yet. 
