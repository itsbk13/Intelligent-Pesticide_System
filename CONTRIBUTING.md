## 🤝 Contributing

To advance precision agricultural research:

1. **Fork** the repository
2. **Create** a feature branch `git checkout -b feature/AmazingFeature`
3. **Commit** your changes `git commit -m 'Add AmazingFeature'`
4. **Push** to the branch `git push origin feature/AmazingFeature`
5. **Open** a Pull Request

### Areas for Contribution:

- **New Crop Types**: Extend models to additional agricultural crops
- **Advanced Architectures**: Implement cutting-edge deep learning models
- **Economic Models**: Enhance cost-benefit analysis frameworks
- **Visualization**: Improve results presentation and dashboards


## 🚀 Quick Start

### Installation:

```bash
# Clone repository
git clone https://github.com/itsbk13/intelligent-pesticide-system.git
cd intelligent-pesticide-system

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Run Research Pipeline:

```bash
# Start with environment setup
jupyter notebook notebooks/01_environment_setup.ipynb

# Follow the complete pipeline:
02_data_preparation.ipynb → 03_data_augmentation.ipynb → 04_model_architecture.ipynb →
05_training_pipeline.ipynb → 06_spray_decision_system.ipynb → 07_evaluation_testing.ipynb
```

### Quick Demo:

```python
# Quick Demo - Load and test trained models
import torch
import segmentation_models_pytorch as smp

# Load best model (100% accuracy)
model = smp.DeepLabV3Plus(encoder_name="resnet50", classes=4)
model.load_state_dict(torch.load('models/trained/DeepLabV3Plus-ResNet50_trained.pth'))
model.eval()

# Run inference demo
jupyter notebook notebooks/08_inference_demo.ipynb
```
