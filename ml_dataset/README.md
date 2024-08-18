The dataset used in this project is derived from web traffic data collected by SNARE sensors over several years, with annotations based on regular expressions to identify various types of web-based attacks. 

This dataset includes four primary types of attacks: 
-	SQL Injection (SQLi): Malicious SQL queries are injected into input fields to manipulate databases
-	Cross-Site Scripting (XSS): Attackers inject malicious scripts into web pages viewed by other users
-	Local File Inclusion (LFI): Exploits vulnerabilities to access files on the server
-	Remote File Inclusion (RFI): Allows attackers to include remote files on a web server
-	Index: Normal, benign web requests

To enhance the dataset's robustness and reduce noise and imbalance, supplementary data from external cybersecurity repositories were integrated. The dataset is constructed with 67 features extracted from URLs, followed by preprocessing steps such as label encoding, TF-IDF transformation on a character level, and meticulous cleaning to remove duplicates, address missing values, and eliminate outliers. Despite the imbalanced nature of the dataset, with a higher proportion of normal traffic, it serves as a robust foundation for developing a machine learning-based classifier intended to replace the existing regular expression-based detection in TANNER, aiming for improved accuracy and lower latency in real-time web attack detection. 


Entire Dataset Class Distribution
<img width="192" alt="Screenshot 2024-08-16 at 12 51 11 PM" src="https://github.com/user-attachments/assets/f7a3737e-0a3e-42ad-a701-317c243da1a5">

Train Set Statistics: 

Test Set Statistics: 

- Label 0: Index
- Label 1: LFI 
- Label 2: RFI
- Label 3: SQLi
- Label 4: Unknown
- Label 5: XSS

External Datasets Used:

- [XSS Payload List - Cross Site Scripting Vulnerability Payload List](https://www.kitploit.com/2018/05/xss-payload-list-cross-site-scripting.html)
- [Deep-XSS](https://github.com/das-lab/deep-xss/blob/master/xssed.csvl)
- [RFI Payloads](https://github.com/infosec-au/fuzzdb/blob/master/attack-payloads/rfi/rfi.txt)
- [XSS-attack-detection](https://github.com/shalayiding/XSS-attack-detection-using-deep-learning/blob/main/XSS_dataset_mixed.csv)
- [Cross site scripting XSS dataset for Deep learning](https://www.kaggle.com/datasets/syedsaqlainhussain/cross-site-scripting-xss-dataset-for-deep-learning)
- [XSS Payload List](https://github.com/payloadbox/xss-payload-list/blob/master/Intruder/xss-payload-list.txt)
- [LFI Payloads](https://raw.githubusercontent.com/emadshanab/LFI-Payload-List/master/LFI%20payloads.txt)
- [SQL Injection Dataset](https://www.kaggle.com/datasets/sajid576/sql-injection-dataset)
- [sql injection dataset](https://www.kaggle.com/datasets/syedsaqlainhussain/sql-injection-dataset)
- [SQL-Injection-Detection](https://github.com/saptajitbanerjee/SQL-Injection-Detection)
- [Malicious And Benign URLs](https://www.kaggle.com/datasets/siddharthkumar25/malicious-and-benign-urls)
