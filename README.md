# Radar Signal Deinterleaving 📡

## About
Implementation of radar signal deinterleaving pipeline based on 
Chen et al., IET Radar Sonar Navigation 2023.

During my internship at Bharat Electronics Limited (BEL), I worked 
on a similar radar signal deinterleaving system. This project 
demonstrates the key concepts I implemented there.

## Results
- **Model Accuracy: 100%**
- Radar types classified: 5
- Total pulses processed: 250
- Algorithm: Random Forest Classifier

## Pipeline Steps
1. Generate synthetic PDW (Pulse Descriptor Word) data
2. Convert PDW data to HSV dot matrix images
3. Train Random Forest classifier
4. Segment each radar type
5. Map back to original PDW format
6. Evaluate with confusion matrix

## 5 Radar Types Implemented
| Type | Name | Description |
|------|------|-------------|
| Type 1 | PRI Constant | Regular pulse timing |
| Type 2 | PRI Jittered | Random timing variations |
| Type 3 | PRI Staggered | Alternating intervals |
| Type 4 | Frequency Agile | Random frequency jumps |
| Type 5 | Group-Group FAR | Group frequency jumps |

## Tech Stack
- Python 3.11
- NumPy
- OpenCV
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Reference
Chen, T., et al. "A novel deinterleaving method for radar pulse 
trains using pulse descriptor word dot matrix images and 
cascade-recurrent loop network." 
IET Radar, Sonar & Navigation 17.11 (2023): 1626-1638.

## Author
K T Tanuja | ML Engineer | Bangalore
github.com/tanuja1229