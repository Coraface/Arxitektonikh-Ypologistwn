## Εργασία 1

### <b> Ερώτημα 1)</b>  
Στην αρχή της κλάσης και στην main() παρατηρώ:  
  1. _Μέγεθος cache μνήμης_  
    `cache_line_size = 64` : Τίθεται fixed 64 bytes στην αρχή της κλάσης   
  2. _Τύπος CPU_  
    `parses.add_argument("--cpu",...)` : Βy default βλέπω ότι τίθεται atomic, εκτός αν περάσω κάποιον άλλο τύπο μέσω --cpu  
  3. _Συχνότητα λειτουργίας_  
    `parses.add_argument("--cpu-freq",...)` : By default βλέπω ότι τίθεται _4Ghz_  
  4. _Αριθμός πυρήνων_  
    `parses.add_argument("--num-cores",...)` : By default τίθεται _1_ πυρήνας  
  5. _Τύπος μνήμης_  
    `parses.add_argument("--mem-type",...)` : By default _DDR3_1600_8x8_  
  6. _Μέγεθος φυσικής μνήμης_  
    `parses.add_argument("--mem-size",...)` : By default _2GB_  
  7. _Αριθμός Memory Channels_  
    `parses.add_argument("--mem-channels",...)` : By default _2_  
  8. _Αριθμός Memory Ranks per Channel_  
    `parses.add_argument("--mem-ranks",...)` : By default _None_
    <br><br>
### <b> Ερώτημα 2)</b>  
Στο config.ini παρατηρώ  
  1. _Μέγεθος cache μνήμης και Μέγεθος φυσικής μνήμης_  
    [system]  
   `cache_line_size = 64`
   `mem_ranges=0:2147483647`  
  2. _Τύπος CPU και αριθμός Threads_
   [system.cpu_cluster.cpus]  
   `type=MinorCPU`
   `numThreads=1`  
  3. _Αριθμός Memory Ranks per Channel_
   [system.mem.ctrls0]
   `ranks_per_channel=2`
