The repository reflects the full research process, with different model versions corresponding to different stages of experimentation and design evolution.

## Model Evolution

This project follows an iterative research workflow:

1. **Baseline Models**  
   Initial experiments with XceptionNet-based architectures.

2. **Architecture Improvements**  
   Exploration of attention mechanisms (CBAM) and enhanced feature extraction.

3. **Frequency-Domain Features**  
   Introduction of FFT-based models to capture manipulation artifacts not visible in spatial domain.

4. **Final Model (Dual-Branch)**  
   Combination of spatial and frequency-domain features to improve robustness and generalization.

## Key Trade-off

A major design decision in this project was balancing model complexity and generalization performance.  

While improving spatial feature extraction alone provided limited gains, incorporating frequency-domain features introduced additional complexity but significantly improved robustness. The final dual-branch design reflects a balance between performance and computational cost.

## Tech Stack

- Python
- PyTorch
- OpenCV
- NumPy / SciPy

## Notes

This repository contains multiple model versions and experimental scripts, reflecting the iterative process of model design and optimization.
