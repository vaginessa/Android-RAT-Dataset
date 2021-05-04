# Android-RAT-Dataset
<h4 align="center">This repo contains all dataset for my research/analysis about : <br>
"DETEKSI REMOTE ACCESS TROJAN PADA ANDROID BERBASIS PENGAMATAN LALU LINTAS JARINGAN <br> MENGGUNAKAN MACHINE LEARNING." </h4>

---on going.....

# Apps Name
| Name | Label |
| ---------- | ---------- |
| AhMyth | Trojan |
| AndroidRAT | Trojan |
| AndroidTester | Trojan |
| DroidJack | Trojan |
| HawkShaw | Trojan |
| SpyMax | Trojan |
| Google | Benign |
| Facebook | Benign |
| Twitter | Benign |

# DATA SET 1 FEATURES
| Name | Desc |
| ----------- | ------------ |
| Source | The port number of source packet |
| Destination | The port number of destination packet |
| Protocol | The type protocol used in packet |
| Length | The size of data generated by the packet (Byte) |
| Type | Type of packet - In or Out |
| Duration | The duration between previous package to the next packet (Second) |

# DATA SET 2 FEATURES
| Name | Desc |
| ------------- | ------------ |
| Total Length Out | The amount of data size generated by packet out of 20 mixed packet (Byte) |
| Total Length In | The amount of data size generated by packet in of 20 mixed packet (Byte) |
| Avg Packet Length Out | The average data size generated by packets out of 20 mixed packets (Byte) |
| Avg Packet Length In | The average data size generated by incoming packets of 20 mixed packets (Byte) |
| Avg Duration Out | The average duration required by packets out of 20 mixed packets (Second) |
| Avg Duration In | The average duration required by incoming packets from 20 mixed packets (Second) |
| Total Duration | The total duration required by 20 mixed packets (Second) |

# Dataset
|  | Dataset 1 | Dataset 2 |
| ----- | ---- | ---- |
| Training | 14400 | 5400 |
| Testing | 3600 | 600 |
| Total | 18000 | 6000 |

*note : raw/original dataset contains more row perpcap rat

# Accuracy and Machine Learning Algorithm Used
| Dataset 1 | Decision Tree | Random Forest | Naive Bayes |
| ------------ | ---------- | ---------- | ---------- |
| N900 - RAT90 | 0.9989 | 0.9990 | 0.1181 |
| N1800 - RAT90 | 0.9994 | 0.9989 | 0.0756 |
| N1800 - RAT1800 | 0.9997 | 0.9997 | 0.4691 |

| Dataset 2 | Decision Tree | Random Forest | Naive Bayes |
| ------------ | ---------- | ---------- | ---------- |
| N150 - RAT10 | 0.873 | 0.933 | 0.513 |
| N300 - RAT10 | 0.883 | 0.929 | 0.545 |
| N300 - RAT300 | 0.90 | 0.928 | 0.71 |

*note : accuracy based on jupyter python result

# Source Original Dataset
Name : Android Mischief Dataset v1<br>
Author : <b>Kamila Babayeva</b>, Stratosphere Laboratory<br>
Date : November 18th 2020<br>
URL : https://www.stratosphereips.org/android-mischief-dataset
