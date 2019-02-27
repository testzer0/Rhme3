# Rhme3

rhme3.elf is the executable. sploit2.py is the exploit. Uses offsets harcoded to my system.

# Synopsis

1) UAF on deleting object : still remains selected if previously selected.

2) Alloc enough smallbin size objects to trigger use of Unsorted bin and use UAF to leak libc.

3) Use UAF to overwrite free hook with addr of system and spawn shell.
