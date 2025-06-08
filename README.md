# Aswin_Harish_Major-Adversarial-Attack-on-Deep-Learning-Model-Detecting-SQli
## **Overview** 
SQL Injection (SQLi) remains one of the most critical security threats to web applications, enabling malicious actors to manipulate backend SQL queries by injecting crafted input into vulnerable fields. These attacks can lead to unauthorized data access, data corruption, or even full system compromise depending on the privileges of the exploited query.

In this project, we develop a model to detect SQLi payloads using a deep learning model. The goal is to degrade the model’s ability to accurately classify malicious SQL inputs by generating adversarial examples that are misclassified as benign, while still executing successfully on the target application (DVWA) and achieving the intended malicious effect on the backend in terms of manipulation or inserting a malicious script .Conventional machine learning models often fail to detect adversarial inputs — carefully modified payloads designed to bypass detection by subtly altering the input without breaking its functionality. To address this, we explore the generation of adversarial SQLi payloads through character-level and token-level perturbations. These adversarial examples simulate real-world evasion techniques, such as string obfuscation, case manipulation, whitespace injection, or comment-based splitting, which attackers often use to circumvent pattern-based detection systems.

The project assess the model’s performance on both standard and adversarial SQLi inputs. The insights gained from these experiments expose weaknesses in the detection model and emphasize the importance of adversarial training in enhancing the robustness of security models against evolving SQLi threats.

-----
## **Key Features**  
- **Deep Learning Detection**:Light weight LSTM based deep learnig model meant for learning SQL syntaxes and queries from a character level
- **Adversarial Attack Generation**: Creation of adversarial SQLi payloads based on string obfuscation,dummy conditions, case manipulation, whitespace injection and comment-based splitting in combination.
- **Model Evaluation**: Model performance is tested against both normal and adversarial payloads to assess robustness.
- **Performance Impact Analysis**: Identifying the impact of perturbation across Precision,Recall,F1-Score,Detection Rate,Accuracy and Escape Rate.
------
# **Setup Instructions**
## Prerequisites
Ensure you have the following installed:

- **Python**: Version 3.8 or higher(Ideally the latest Version 3.12)
- **TensorFlow**: Version 2.16 
## Required Libraries

Install the following libraries before running the project:

- **NumPy**  
- **Pandas**
- **sqlparse**
- **Scikit-learn**  
- **Matplotlib**  
- **Jupyter Notebook**  
- **VS Code Extensions**:
  - **Python** (for Python environment support)  
  - **Jupyter** (for running notebooks in VS Code)
 
You can install them using:

```bash
pip install numpy pandas scikit-learn matplotlib jupyter sqlparse
```
--------
