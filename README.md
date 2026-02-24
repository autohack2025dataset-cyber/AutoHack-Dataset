# AutoHack Dataset

A high-fidelity vehicular cybersecurity dataset collected from a modern production vehicle under real-world driving conditions.

The dataset provides synchronized multi-CAN bus logs and includes advanced attack scenarios such as UDS-based diagnostics manipulation and timing-aware Replay attacks. Attack impacts were physically verified to ensure reliable ground-truth labeling, including safety-related vehicle responses observed during controlled injections.

Benchmark evaluations indicate that this dataset presents a significant challenge to existing intrusion detection systems and supports reproducible cybersecurity research in automotive environments.

This repository is anonymized for double-blind peer review.

---

## Dataset Download


**Download link :**  
https://drive.google.com/drive/folders/1BIFxQCkWdfiiM5DpMYH6AKzPVcBSTcqL?usp=sharing

---

## File Structure

The dataset is organized as follows:
Interface/
Train/
Test/

### 📁 Interface

Contains datasets with an additional `interface` column indicating the originating CAN bus for each message.  
This enables **multi-bus** analysis and cross-domain intrusion detection research.

### 📁 Train

Training dataset without the `interface` column.  
The bus information is excluded to simulate a standard IDS training environment.


### 📁 Test

Test dataset without the `interface` column.  
Maintains the same structure as the Train dataset for fair evaluation.
