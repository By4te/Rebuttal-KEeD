# Answer to Reviewer KEeD

## Additional experiments conducted on the sleep stage datasets

Table 1. A summary of the SHHS dataset
| Dataset | Subjects | EEG Channel | EOG Channel | Scoring Rule | Sampling Rate |
|---------|----------|-------------|-------------|--------------|---------------|
| SHHS[1] | 329      | C4-A1       | ROC-LOC     | R&K          | 125 Hz        |

Table 2. Performance comparison between ConfSleepNet and state-of-the-art methods for automatic sleep staging. The best results are highlighted in bold.

![2](https://github.com/user-attachments/assets/1ebc333d-4adc-4c5d-a3ad-7997c25bc4bb)


## Performance comparison

Table 3. Comparison with low-quality modality fusion / uncertainty-aware sleep staging methods on multiple public datasets

<img width="410" height="340" alt="image" src="https://github.com/user-attachments/assets/65e97ae4-523f-4b25-8bc4-ee2979ebc47c" />

## Additional experiments conducted on the multi-view datasets

Table 4. Summary of multi-view datasets 

| Dataset    | View | Class | Size  |
|------------|------|-------|-------|
| HandWritten| 6    | 10    | 2000  |
| Scene15    | 3    | 15    | 4485  |
| CUB        | 2    | 200   | 11788 |
| PIE        | 3    | 68    | 680   |

HandWritten: https://archive.ics.uci.edu/dataset/72/multiple+features 

Scene15: https://figshare.com/articles/dataset/15-Scene_Image_Dataset/7007177/1 

CUB: https://www.vision.caltech.edu/visipedia/CUB-200.html 

PIE: http://www.cs.cmu.edu/afs/cs/project/PIE/MultiPie/Home.html

Table 4. Performance comparison on multi-view datasets.
| Dataset     | EDL[12]      | DCCAE[13]    | CAML[14]     | ETMC[15]     | RCML[16]     | CCML[17]     | TMCEK[18]    | CMAM (Ours) |
|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|
| HandWritten | 97.00±0.16  | 97.05±0.24  | 98.10±0.12  | 98.32±0.22  | 98.70±0.19  | 98.75±0.27  | 97.75±0.42  | 98.45±0.58  |
| Scene15     | 60.60±0.13  | 64.26±0.42  | 70.17±0.13  | 66.87±0.29  | 71.28±0.32  | 72.60±0.87  | 71.06±0.87  | 73.01±1.09  |
| CUB         | 89.51±0.24  | 85.39±1.36  | 94.33±0.73  | 91.05±0.63  | 93.28±2.75  | 94.58±1.30  | 90.50±2.51  | 95.00±2.32  |
| PIE         | 87.99±0.56  | 81.96±1.04  | 93.38±0.80  | 93.82±0.82  | 93.89±2.46  | 94.56±1.83  | 95.15±2.81  | 95.74±1.80  |

## Uncertainty Evaluation

<img width="1920" height="973" alt="PIE" src="https://github.com/user-attachments/assets/c70c9f1b-4d9d-4e73-9b4a-1eb85896ef51" />

Figure 1. Density of uncertainty on the PIE dataset. As the noise intensity increases, the uncertainty curves of conflicting instances also increase.

<img width="1200" height="964" alt="hand" src="https://github.com/user-attachments/assets/5202e082-90a0-4446-a628-5a7b56b00744" />

Figure 2. Density of uncertainty on the Handwritten dataset.


## Reference

[1] Zhang, G., Cui, L., Mueller, R., Tao, S., Kim, M., Rueschman, M. N., Mariani, S., Mobley, D., and Redline, S. The national sleep research resource: towards a sleep data commons. Journal of the American Medical Informatics Association, 25:1351 – 1358, 2018.

[2] Supratak, A., Dong, H., Wu, C., and Guo, Y. DeepSleepNet: a model for automatic sleep stage scoring based on raw single-channel EEG. IEEE Transactions on Neural Systems and Rehabilitation Engineering, 25(11):1998–2008, 2017.

[3] Supratak, A. and Guo, Y. TinySleepNet: An efficient deep learning model for sleep stage scoring based on raw single-channel EEG. In 42nd Annual International Conference of the IEEE Engineering in Medicine & Biology Society, pp. 641–644, 2020.

[4] Jia, Z., Lin, Y., Wang, J., Wang, X., Xie, P., and Zhang, Y. SalientSleepNet: multimodal salient wave detection network for sleep staging. arXiv preprint: 2105.13864, 2021.

[5] Phan, H., Chen, O. Y., Tran, M. C., Koch, P., Mertins, A., and De Vos, M. XSleepNet: Multi-view sequential model for automatic sleep staging. IEEE Transactions on Pattern Analysis and Machine Intelligence, 44(9):5903–5915, 2022.

[6] Lee, S., Yu, Y., Back, S., Seo, H., and Lee, K. SleePyCo: automatic sleep scoring with feature pyramid and contrastive learning. Expert Systems with Applications, 240: 122551, 2024.

[7] Ren, Z., Ma, J., and Ding, Y. FlexibleSleepNet: A model for automatic sleep stage classification based on multi-channel polysomnography. IEEE Journal of Biomedical and Health Informatics, 29(5): 3488-3501, 2025.

[8] Liang, X., Wang, S., Qian, Y., Guo, Q., Du, L., Jiang, B., Luo, T., and Li, F. Trusted multi-view classification with expert knowledge constraints. In International Conference on Machine Learning, 2025.

[9] Wang, K., Zhu, Q., Zhao, J., Zheng, C., Shao, W., and Zhang, D. Heterogeneous modality dynamic trustworthy fusion network for cross-subject sleep stage classification. IEEE Transactions on Emerging Topics in Computational Intelligence, 2026.

[10] Huang, G., and Ma, F. Trustsleepnet: A trustable deep multimodal network for sleep stage classification. In IEEE-EMBS International Conference on Biomedical and Health Informatics, 2022.

[11] Hu, S., Wang, Y., Liu, J., and Yang, C. Xsleepfusion: A dual-stage information bottleneck fusion framework for interpretable multimodal sleep analysis. Information Fusion, 123: 103275, 2025.

[12] Sensoy, M., Kaplan, L., and Kandemir, M. Evidential deep learning to quantify classification uncertainty. In Advances in Neural Information Processing Systems,  volume 31, pp. 3179-3189, 2018.

[13] Wang, W., Arora, R., Livescu, K., and Bilmes, J. On deep multi-view representation learning. In International Conference on Machine Learning, pp. 1083-1092, 2015.

[14] Zhou, H., Xue, Z., Liu, Y., Li, B., Du, J., Liang, M., and Qi, Y. Calm: An enhanced encoding and confidence evaluating framework for trustworthy multi-view learning. In Proceedings of the ACM International Conference on Multimedia, pp. 3108-3116, 2023.

[15] Han, Z., Zhang, C., Fu, H., and Zhou, J. T. Trusted multiview classification with dynamic evidential fusion. IEEE Transactions on Pattern Analysis and Machine Intelligence, 45(2):2551-2566, 2023.

[16] Xu, C., Si, J., Guan, Z., Zhao, W., Wu, Y., and Gao, X. Reliable conflictive multi-view learning. In Proceedings of the AAAI Conference on Artificial Intelligence, volume 38, pp. 16129-16137, 2024.

[17] Liu, Y., Liu, L., Xu, C., Song, X., Guan, Z., and Zhao, W. Dynamic evidence decoupling for trusted multi-view learning. In Proceedings of the ACM International Conference on Multimedia, pp. 7269-7277, 2024.

[18] Liang, X., Wang, S., Qian, Y., Guo, Q., Du, L., Jiang, B., Luo, T., and Li, F. Trusted multi-view classification with expert knowledge constraints. In International Conference on Machine Learning, 2025.
