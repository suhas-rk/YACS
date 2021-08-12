# Yet Another Centralized Scheduler (YACS)

---

This repository contains code and report for the project Yet Another Centralized Scheduler (YACS) for the course UE18CS322 - Big Data by the team BD_0054_0186_1555_1965 consisting of:

Suhas R. [PES1201800186] 
Harish S [PES1201801965]  
Vikshith Shetty [PES1201801555]  
Prateek Nayak [PES1201800054]  

---
### Dependencies

* The core Master Worker pair doesn't have any external dependencies other than the standard libraries shipped with Python 3.7+  
* The Analytics portion uses Matplotlib to plot the graph as an external dependency

---

### Instruction to run the program

Clone this repository and execute the following commands to do a dry run to get analytics

```bash
cd yacs
./run.sh
cd analytics
python3 analysis.py
```

If you want to run only the master worker pair, first modify the config file and then run

```bash
./star-all.sh
```
to run all the workers at specific ports.  
To run master execute
```bash
python3 master.py --sa={round-robin,least-loaded,random}
```

The argument `sa` is used to select the scheduling algorithm

---

This implementation of YACS was tested majorly on Linux.  

---

Thank you for going through this document. You can find the report of our findings in BD_0054_0186_1555_1965.pdf present at top level of this repository

---