##keep running
Kepp a script or bash cmd running. Relaunch the command or script when exit.

##installation
```bash
pip install keep-running
```

##usage

For example: `test-program.sh`

```bash
#!/bin/bash
for i in {1..10}
do
    echo `date` ':' $i
    sleep 1
done
```

```bash
keep-running test-program.sh
```

The log file will be: `test-program.sh.log` in the same directory with `test-program.sh`.

Tips: The file used to lock is `test-program.sh.lock`.


