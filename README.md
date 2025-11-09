Switch this repo to run on mac with python only instead (was config to compile to an exe to run on windows)

Issues:
- old code not working at all despite manually installing all the packages with respective versions

To-dos:
- switch to use python venv instead of peotry temporarily for easily set up

Progress:
- create a virtual env temporarily
- working on making in run
- comment all the unneeded modules for now
- block 1
- reread main code, seems like gui.py is needed no matter what
- block 2
- block 3
- look at whole flow before cont further
  - make a map of the flow with excalidraw

Blocks:
1. in venv, after commenting gui.py, it is still somewhat called when calling main.py (solved: installed missing modules)
2. No module named '_tkinter' (solved: brew install python-tk@3.14)
3. python keep crashes after pysimplegui is working (solution: go with FreeSimpleGUI or Pyside6)

Solution trial for blocks:
3. 
- debug, error pops as soon as step into importing PysimpleGUI
- tried running a seperate file by importing PySimpleGUI, seems like a lot of the functions are not working
- looking at PySimpleGUI module, turns out PySimpleGUI has shut down its free version completely, seems like the author is not happy his code is not generating any monies! looking into alternatives for PySimpleGUI
