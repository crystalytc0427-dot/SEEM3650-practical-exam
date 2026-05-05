%%writefile report.md
# SEEM3650 Practical Exam Report
**Student ID:** 1155214043 (XYZ=043)  
**Iterations used:** 400 (consistent across all runs)

## Step 2 – Shakespeare samples (first 5 lines)
The mento heavens, to that I me my held
What griene senge will is the loves, and the not on that theirs not
The the he country: the haves hew you love up.
But and good not my would that
To Willongue Cerians to them such a peopience of the ence.

## Step 3 – Model architecture (vary layers, fixed heads=4)
### Validation loss at iteration 400:
- n_layer=2: No val loss found
- n_layer=3: 1.8394
- n_layer=5: 1.8209
- n_layer=7: 1.8206

Lowest validation loss: **1.8206** (n_layer=7) or 1.8209 (n_layer=5) – values are very close.

### Plot
![layers vs loss](figures/layers_vs_loss.png)

### Best settings
Lowest validation loss = 1.8206 with n_layer = 7 and n_head = 4.

## Step 4 – Code generation (Python)
### Token count from prepare.py:
Train tokens: 4,825,115  
Val tokens: 536,124

### First 20 lines of generated samples:
Overriding: out_dir = out-code-gen
Overriding: start = def 
Overriding: num_samples = 1
Overriding: max_new_tokens = 800
number of parameters: 10.72M
Loading meta from data/code_generation/meta.pkl...
def f  f afomat id = oooan ate t soope_byt + Ta tring_thane mewithe ad coubackmachare at % de tut wrerth con ted f bach s te] all t tpi it ion ad Tasit who Tumat  ath as as e a (
                                                                                                                                                                                                           "s((
                                                               y                                                                                                                                       "                                     ut                                                "   "f"                           """
        "  ", 1095696051406).                                   "== "a"""\',
               
---------------
### Favorite generated snippet           
   y                                                                                                                                       "                                     ut                                                "   "f"                           """
        "  ", 1095696051406).                                   "== "a"""\',
