# DeepCOP

1. Download and uncompress the level 5 gctx data files and experiment metadata from GEO
   * Phase 1: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE92742
     * GSE92742_Broad_LINCS_Level5_COMPZ.MODZ_n473647x12328.gctx.gz <br>
     * GSE92742_Broad_LINCS_sig_info.txt.gz <br>
   * Phase 2: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE70138 <br>
     * GSE70138_Broad_LINCS_Level5_COMPZ_n118050x12328_2017-03-06.gctx.gz <br>
     * GSE70138_Broad_LINCS_sig_info_2017-03-06.txt.gz <br>

2. The morgan descriptor files in the Data folder are large so they had to be compressed to github. Uncompress these files in the same folder. 

3. Use [get_xy.py](get_xy.py) or [get_xy_phase2.py](get_xy_phase2.py) to collect the training data and labels.

4. Use [internal_validation.py](internal_validation.py) to do 10 fold cross validation on the training data.

5. Use [external_validation.py](external_validation.py) to evaluate predictions from step 3 trained models on external RNA-Seq values.
