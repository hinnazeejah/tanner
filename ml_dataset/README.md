The dataset used in this project is derived from web traffic data collected by SNARE sensors over several years, with annotations based on regular expressions to identify various types of web-based attacks. 

This dataset includes four primary types of attacks: 
-	SQL Injection (SQLi)  Malicious SQL queries are injected into input fields to manipulate databases
-	Cross-Site Scripting (XSS)  Attackers inject malicious scripts into web pages viewed by other users
-	Local File Inclusion (LFI)  Exploits vulnerabilities to access files on the server
-	Remote File Inclusion (RFI)  Allows attackers to include remote files on a web server
  
Index  Normal, benign web requests.

To enhance the dataset's robustness and reduce noise and imbalance, supplementary data from external cybersecurity repositories were integrated. The dataset is constructed with 67 features extracted from URLs, followed by preprocessing steps such as label encoding, TF-IDF transformation on a character level, and meticulous cleaning to remove duplicates, address missing values, and eliminate outliers. Despite the imbalanced nature of the dataset, with a higher proportion of normal traffic, it serves as a robust foundation for developing a machine learning-based classifier intended to replace the existing regular expression-based detection in TANNER, aiming for improved accuracy and lower latency in real-time web attack detection. 

