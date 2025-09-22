# asm-labs

## Problem
Understand how Linux manages memory and how malloc works under the hood.

## Approach
1. Observe '/proc/meminfo' and 'vmstat'.
2. Trace 'malloc' and 'free' with 'strace'.
3. Implement a tiny malloc using 'sbrk'.

## Result
- Verified that malloc uses both 'brk' and 'mmap' depending on allocation size.
- Confirmed memory statistics change in '/proc/meminfo'.

## Reproduce
'''bash

make
./01_meminfo/run.sh
./02_malloc_trace/run.sh
