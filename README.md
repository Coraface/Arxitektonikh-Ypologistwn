## Εργασία 1

### <b> Ερώτημα 1)</b>  
Στην αρχή της κλάσης και στην main() παρατηρώ:  
  1. _Μέγεθος cache μνήμης_  
    `<cache_line_size = 64>` : Τίθεται fixed 64 bytes στην αρχή της κλάσης   
  2. _Τύπος CPU_  
    `<parses.add_argument("--cpu",...)>` : Βy default βλέπω ότι τίθεται atomic, εκτός αν περάσω κάποιον άλλο τύπο μέσω --cpu  
  3. _Συχνότητα λειτουργίας_  
    `<parses.add_argument("--cpu-freq",...)>` : By default βλέπω ότι τίθεται 4Ghz  
  4. _Αριθμός πυρήνων_  
    `parses.add_argument("--num-cores",...)` : By default τίθεται 1 πυρήνας  
  5. _Τύπος μνήμης_  
    `<parses.add_argument("--mem-type",...)>` : By default DDR3_1600_8x8  
  6. _Μέγεθος φυσικής μνήμης_  
    `<parses.add_argument("--mem-size",...)>` : By default 2GB  
    <br><br>
<b> Ερώτημα 2)</b>  
Στο config.ini παρατηρώ  
  1. _Μέγεθος cache μνήμης και Μέγεθος φυσικής μνήμης_  
    [system]  
   `<cache_line_size = 64>`
   `<mem_ranges=0:2147483647>`
