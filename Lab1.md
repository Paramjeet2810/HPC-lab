# Important comands for this lab
`lscpu`
This command is suitable for linux machines only.

`gprof`
This command is used for profiling of the code. Use the following steps to execute the command.
1. Compile the code with an extra flag `-pg`.

```bash
gcc lab1.c -o lab1 -pg
```
  
2. Run the code   
  ```bash
  ./lab1
  ```
  
3. Perform an ls and you would find a file named gmon.out. To understand the fileuse the following command

  ```bash
  gprof -b lab1 gmon.out
  ```  
  `-b` is the flag used to make things laconic. If you wish to understand the meaning of each line in the output of the command run the code without the flag.
