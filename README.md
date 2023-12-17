"**PACHA: Pairwise Chemical Graph Alignment Software** 

**Overview:** PACHA is a software tool for aligning chemical graphs.

**Description:** PACHA aligns two chemical compounds represented as small graphs, producing an atom-atom mapping between them. This alignment can be used to create feature vectors for machine learning applications, such as support vector machines. Key use cases include metabolic pathway reconstruction and virtual screening [1].

**Demo:** To use PACHA, navigate to the 'pacha/src' directory, run 'make,' and execute './pacha --input_file=../dat/target_compounds/ --output_file=output.txt.' The 'output.txt' file will contain alignment results for all pairs of chemical graphs in '../dat/target_compounds/'.

**Requirements:** 
- GNU C++ compiler (Higher versions are preferable for multi-threading).

**Usage:** 
```
./pacha --input_file=string --output_file=string [options] ...
options:
  -i, --input_file     input file name (string)
  -o, --output_file    output file name (string)
  -d, --dist           maximum distance for computing vertex features (unsigned long long [=5])
  -k, --topk           number of alignments starting from vertex pairs of top-k matching scores (unsigned long long [=10])
  -n, --num_threads    number of threads (unsigned long long [=1])
  -t, --threshold      threshold (float [=0])
  -c, --inter_cuts     maximum number of intermolecular cuts (unsigned long long [=100000000])
  -a, --intra_cuts     maximum number of intramolecular cuts (unsigned long long [=100000000])
  -?, --help           print this message
```

**Installation:** To install PACHA, navigate to the 'pacha/src' directory and run 'make.'

**License:** New BSD License

**Author:** Yasuo Tabei (yasuo.tabei@gmail.com)  
[Homepage](https://sites.google.com/site/yasuotabei/)  
[tb-yasu](https://github.com/tb-yasu)

**Reference:** [1] Yoshihiro Yamanishi*, Yasuo Tabei*, Masaaki Kotera: Metabolome-scale de novo pathway reconstruction using regioisomer-sensitive graph alignments, In Proceedings of ISMB/ECCB, 2015. (*joint first author)"
