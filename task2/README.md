## Εργασία 2 - Φοιτητές: Χωραφάς Χρήστος(8718)/Φάββας Αντώνης(8675), Ομάδα 33

### <pre><b> Βήμα 1)</b></pre>  
#### <b>Ερώτημα 1</b>  
_Benchmark 401_:  
  1. _`i_cache_size : 32768`_  
  2. _`i_cache_assoc : 2`_  
  3. _`d_cache_size : 65596`_  
  4. _`d_cache_assoc : 2`_  
  5. _`l2_size : 2097152`_    
  6. _`l2_assoc : 8`_    
  7. _`cache_line_size : 64`_  
    <br><br>
    
_Benchmark 429_:  
  1. _`i_cache_size : 32768`_  
  2. _`i_cache_assoc : 2`_  
  3. _`d_cache_size : 65536`_  
  4. _`d_cache_assoc : 2`_  
  5. _`l2_size : 2097152`_    
  6. _`l2_assoc : 8`_    
  7. _`cache_line_size : 64`_  
    <br>
    
_Benchmark 456_:  
  1. _`i_cache_size : 32768`_  
  2. _`i_cache_assoc : 2`_  
  3. _`d_cache_size : 65596`_  
  4. _`d_cache_assoc : 2`_  
  5. _`l2_size : 2097152`_    
  6. _`l2_assoc : 8`_    
  7. _`cache_line_size : 64`_  
    <br>
    
_Benchmark 458_:  
  1. _`i_cache_size : 32768`_  
  2. _`i_cache_assoc : 2`_  
  3. _`d_cache_size : 65596`_  
  4. _`d_cache_assoc : 2`_  
  5. _`l2_size : 2097152`_    
  6. _`l2_assoc : 8`_    
  7. _`cache_line_size : 64`_  
    <br>
    
_Benchmark 470_:  
  1. _`i_cache_size : 32768`_  
  2. _`i_cache_assoc : 2`_  
  3. _`d_cache_size : 65596`_  
  4. _`d_cache_assoc : 2`_  
  5. _`l2_size : 2097152`_    
  6. _`l2_assoc : 8`_    
  7. _`cache_line_size : 64`_  
    <br>
 <pre> Παρατήρηση: όλα είναι ίδια.</pre>
 <br><br>
    
#### <pre><b>Ερώτημα 2</b></pre>  
_Benchmark 401_:  
  1. _`sim_seconds : 0.082631`_  
  2. _`CPI : 1.652621`_  
  3. _`i_misses : 0.000051`_  
  4. _`d_misses : 0.015205`_  
  5. _`l2_misses : 0.281779`_    
    <br>
    
_Benchmark 429_:  
  1. _`sim_seconds : 0.120773`_  
  2. _`CPI : 1.207734`_  
  3. _`i_misses : 0.01037`_  
  4. _`d_misses : 0.001938`_  
  5. _`l2_misses : 0.110032`_    
    <br>
    
_Benchmark 456_:  
  1. _`sim_seconds : 0.058129`_  
  2. _`CPI : 1.162574`_  
  3. _`i_misses : 0.000186`_  
  4. _`d_misses : 0.001673`_  
  5. _`l2_misses : 0.086262`_    
    <br>
    
_Benchmark 458_:  
  1. _`sim_seconds : 0.514664`_  
  2. _`CPI : 10.293277`_  
  3. _`i_misses : 0.000019`_  
  4. _`d_misses : 0.122943`_  
  5. _`l2_misses : 0.999984`_    
    <br>
    
_Benchmark 470_:  
  1. _`sim_seconds : 0.174660`_  
  2. _`CPI : 3.493201`_  
  3. _`i_misses : 0.000103`_  
  4. _`d_misses : 0.060970`_  
  5. _`l2_misses : 0.999940`_  
    
   <br><br>
#### <pre><b> Ερώτημα 3)</b></pre>  

Για όλα τα benchmarks ισχύει:  
  1. _`--cpu-clock=2GHz : system.clock = 1000`_  
  2. _`--cpu-clock=2GHz : system.cpu.clock = 500`_ 
  3. _`--cpu-clock=1GHz : system.clock = 1000`_  
  4. _`--cpu-clock=1GHz : system.cpu.clock = 1000`_
     <br><br>
     
### <pre><b> Βήμα 2)</b>  
<b>Ερώτημα 1</b></pre>
     
   a) 
   1. TimingSimpleCPU  
   <pre>
final_tick                                   43143000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)  
host_seconds                                     0.05                       # Real time elapsed on the host  
host_tick_rate                              882572071                       # Simulator tick rate (ticks/s)  
sim_freq                                 1000000000000                      # Frequency of simulated ticks  
sim_seconds                                  0.000043                       # Number of seconds simulated  
sim_ticks                                    43143000                       # Number of ticks simulated  
   </pre>
   2. MinorCPU  
   <pre>
final_tick                                   36506000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)
host_seconds                                     0.13                       # Real time elapsed on the host
host_tick_rate                              277111912                       # Simulator tick rate (ticks/s)
sim_freq                                 1000000000000                      # Frequency of simulated ticks
sim_seconds                                  0.000037                       # Number of seconds simulated
sim_ticks                                    36506000                       # Number of ticks simulated
   </pre>
   
  b)  
  Kαι ο MinorCPU και ο TimingSimpleCPU αποτελούν μοντέλα In-order CPUs για αυτο βγάζουν παρόμοια αποτελέσματα ως προν τον χρόνο εκτέλεσης
  
  c)  
  
  * Μειώνοντας την συχνότητα ρολογιού παρατηρώ ότι οι χρόνοι αυξάνονται, σε σχέση με το default clock. Αξίζει να σημειωθεί ότι με default clock, το TimingSimpleCPU έχει μικρότερο host_seconds από το MinorCPU, σε αντίθεση με την περίπτωση των 100KHz.  
  * Αλλάζοντας τον τύπο μνήμης παρατηρώ ότι αυξάνεται ο συνολικός χρόνος προσωμοίωσης καθώς υπάρχει αύξηση των αριθμών των ticks.  
  3. TimingSimpleCPU with --cpu-clock=100KHz  
  <pre>
final_tick                               369010000000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)
host_seconds                                     0.98                       # Real time elapsed on the host
host_tick_rate                           377605550311                       # Simulator tick rate (ticks/s)
sim_freq                                 1000000000000                      # Frequency of simulated ticks
sim_seconds                                  0.369010                       # Number of seconds simulated
sim_ticks                                369010000000                       # Number of ticks simulated
  </pre>
  
  4. MinorCPU with --cpu-clock=100KHz  
  <pre>
final_tick                               206330000000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)
host_seconds                                     0.67                       # Real time elapsed on the host
host_tick_rate                           309016775835                       # Simulator tick rate (ticks/s)
sim_freq                                 1000000000000                      # Frequency of simulated ticks
sim_seconds                                  0.206330                       # Number of seconds simulated
sim_ticks                                206330000000                       # Number of ticks simulated
</pre> 

5. TimingSimpleCPU with --mem-type=LPDDR2_S4_1066_1x32 (Χρησιμοποιήσαμε διαφορετικό από το MinorCPU, ώστε να παρατηρηθεί μεγαλύτερη διαφορά σε σχέση με το default mem-type)
<pre>
final_tick                                   51120000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)
host_seconds                                     0.07                       # Real time elapsed on the host
host_tick_rate                              773261384                       # Simulator tick rate (ticks/s)
sim_freq                                 1000000000000                      # Frequency of simulated ticks
sim_seconds                                  0.000051                       # Number of seconds simulated
sim_ticks                                    51120000                       # Number of ticks simulated
</pre>  

6. MinorCPU with --mem-type=HBM_1000_4H_1x64
<pre>
final_tick                                   42302000                       # Number of ticks from beginning of simulation (restored from checkpoints and never reset)
host_seconds                                     0.13                       # Real time elapsed on the host
host_tick_rate                              325940585                       # Simulator tick rate (ticks/s)
sim_freq                                 1000000000000                      # Frequency of simulated ticks
sim_seconds                                  0.000042                       # Number of seconds simulated
sim_ticks                                    42302000                       # Number of ticks simulated
</pre>
<br><br><br>
## Κριτική
Σαν εργασία ήταν πολύ ενδιαφέρουσα. Ήρθαμε σε επαφή με πιο πρακτικά πράγματα, εργαστήκαμε στο terminal (κάτι που μας αρέσει) και ψάξαμε πληροφορίες για το πως να αλλάξουμε παραμέτρους στα commands. Αυτό από μόνο του σου δίνει μια αίσθηση ικανοποίησης όταν τελικά τα πράγματα τρέχουν όπως θες. Μάθαμε αρκετά για τις προσομοιώσεις, τους επεξεργαστές και τις μνήμες, ακόμα και για την ωραιοποίηση του README χρησιμοποιώντας Markdown. Συναντήσαμε ένα μικρό πρόβλημα με το ανέβασμα των αρχείων, εφόσον μετά είδαμε ότι χρειάζονται όλες οι μετρήσεις και έπρεπε να ξανατρέξουμε τις αντίστοιχες εντολές, όπως και με το γεγονός ότι δεν υπήρχαν αρκετές πληροφορίες στο ίντερνετ για InOrder Cpu. Εν ολίγοις ήταν μια ευχάριστη, όχι πολύ δύσκολη εργασία που κάλυπτε αρκετά πράγματα.

      
<b>_Βιβλιογραφία_<b>:  https://cirosantilli.com/linux-kernel-module-cheat/?fbclid=IwAR3h1ny5hRoVUIGP1vtOsUAzqXYd69sHBAopwuveHZtTSbd_MFp0B4Nmp8c#gem5-cpu-types  
http://gem5.org/InOrder  
http://www.m5sim.org/SimpleCPU#BaseSimpleCPU  
http://www.gem5.org/docs/html/minor.html
