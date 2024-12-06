# Virtual Memory

Why virtual memory?

​	use disk for memory(use RAM as a cache)

​	for memory management

​	isolate address space for different processes	



split into pages: Virtual Page Number + Page offset

### Page Hit:

processorsend virtual address to MMU(memory management unit)

MMU get PTE(Page Table Engtry)

MMU sends physical address to cache/memory

cache/memory sends data to processor

### Page Fault Exception:

when virtual memory reference is not in Physical Memory

valid bit is 0

Page fault handler identifies victim

update PTE in memory

### To speed up translation between VA and PA:

### 	Translation Lookaside Buffer (TLB)

TLB is a small hw cache in MMU

to store page table entries for a small number of pages

VM is split into VPN and Page offset, VPN is split into TLB Tag and TLB Index
