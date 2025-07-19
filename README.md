#  Leveraging MIMIC Datasets for Better Digital Health: A Review on Open Problems, Progress Highlights, and Future Promises


> **Abstract**: The Medical Information Mart for Intensive Care (MIMIC) datasets have become the Kernel of Digital Health Research by providing freely accessible, deidentified records from tens of thousands of critical care admissions, enabling a broad spectrum of applications in clinical decision support, outcome prediction, and healthcare analytics. Although numerous studies and surveys have explored the predictive power and clinical utility of MIMIC based models, critical challenges in data integration, representation, and interoperability remain underexplored. This paper presents a comprehensive survey that focuses uniquely on open problems. We identify persistent issues such as data granularity, cardinality limitations, heterogeneous coding schemes, and ethical constraints that hinder the generalizability and real-time implementation of machine learning models. We highlight key progress in dimensionality reduction, temporal modelling, causal inference, and privacy preserving analytics, while also outlining promising directions including hybrid modelling, federated learning, and standardized preprocessing pipelines. By critically examining these structural limitations and their implications, this survey offers actionable insights to guide the next generation of MIMIC powered digital health innovations.


![mainfig](./Framwork.png)---


![mainfig](./Open_Problems.JPG)---


\begin{table}[!t]
\caption{Key Features and Temporal Granularity in MIMIC Datasets}
\label{tab:mimic_features_temporal}
\centering
\renewcommand{\arraystretch}{1.05}
\begin{tabular}{p{1.3cm} p{2.4cm} p{1.9cm} p{1.0cm}}
\toprule
\textbf{Category} & \textbf{Variable / Dataset} & \textbf{Description} & \textbf{Values / Records} \\
\midrule
%\multirow{4}{*}{\shortstack[l]{High \\Cardinality}} 
& ICD 9 Codes (MIMIC III) & Diagnosis Codes & 14,567 \\
& NDC Codes (MIMIC III) & Medication Identifiers & 4,478 \\
& CPT Codes (MIMIC IV) & Procedure Codes & 5,221 \\
& HADM\_ID (MIMIC III) & Hospital Admissions & 58,976 \\
\midrule
%\multirow{3}{*}{\shortstack[l]{Temporal\\Features}} 
& ICU Chartevents (MIMIC III) & Minute level granularity & 330M+ \\
& Lab Measurements (MIMIC IV) & Hourly to daily & 28M+ \\
& ED Stays (MIMIC IV) & Second-level timestamps & 425K+ \\
\bottomrule
\end{tabular}
\end{table}

## Citation
If you use this framework, please cite our work:

```bibtex
@misc{khaled2025leveragingmimicdatasetsbetter,
      title={Leveraging MIMIC Datasets for Better Digital Health: A Review on Open Problems, Progress Highlights, and Future Promises}, 
      author={Afifa Khaled and Mohammed Sabir and Rizwan Qureshi and Camillo Maria Caruso and Valerio Guarrasi and Suncheng Xiang and S Kevin Zhou},
      year={2025},
      eprint={2506.12808},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2506.12808}, 
}
