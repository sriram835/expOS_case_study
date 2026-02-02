# expOS case study

## Setup:
1. run `git clone https://github.com/sriram835/expOS_case_study`
2. go to xfs-interface folder inside
3. run `./xfs-interface fdisk`. Only do this if you want to execute stages in sequence, because this command erases all data from expOS disk

## Stage 2:
The commands for this stage are given in the OS case study report.pdf, Running the export command will give an error the file already exists.

### Assignment 1:
Run `./xfs-interface dump --rootfile` in xfs-interface folder, and check the rootfile created in xfs-interface folder.

### Assignment 2:
1. Run `./xfs-interface` in xfs-interface folder.
2. Run `dump --inodeusertable`
3. Run `dump --rootfile`
4. Save the rootfile and inodeusertable with different names such as rootfile_before.txt and inodeusertable_before.txt
5. Run `rm sample.dat`
6. Run commands in step 2 and 3 again, and now compare the two new rootfile and inodeusertable with previous files.

## Stage 3:
The commands for this stage are given in the OS case study report.pdf.

### Assignment 1:
The commands for this assignment are given in the OS case study report.pdf.

## Stage 4:
The commands for this stage are given in the OS case study report.pdf.

### Assignment 1:
The commands for this assignment are given in the OS case study report.pdf.

## Stage 5:
1. Run `./xfs-interface load --os ../stage5/oddnos.xsm` in xfs-interface folder.
2. Run `cd ..`
3. Run `cd xsm`
4. Run `./xsm --debug`
- Press `s` to step to next intruction.
- Press `c` to step to next break point.
- Enter `reg` to see register values at a paticular point of execution.

## Stage 6:
1. Go to xfs-interface folder.
2. Run `./xfs-interface load --int=10 ../spl/spl_progs/haltprog.xsm`
3. Run `./xfs-interface load --exhandler ../spl/progs/haltprog.xsm`
4. Run `./xfs-interface load --init ../stage6/squares.xsm`
5. Run `./xfs-interface load --os ../stage6/os_startup.xsm`
6. Go to xsm folder and run `./xsm --debug --timer 0`

- Enter `c` to go to next break point.
- Enter `s` to go to next instruction.
- Enter `reg` see the register values.

### assignment 1:
1. Go to xfs-interface folder.
2. Run `./xfs-interface load --init ../stage6/assignment/squares.xsm`
3. Run `./xfs-interface load --os ../stage6/assignment/os_startup.xsm`
4. Go to xsm folder and run `./xsm --debug --timer 0`


