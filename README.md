# weather-forecast
ML model created for prediction the weather - only for educational purpose !
# Classification Model README

## Overview
This repository contains a machine learning classification model that predicts wether forcast based on past data anf categories based on input data. The model outputs a probability vector, which is then mapped to human-readable labels.

## Installation
To use this model, ensure you have Python installed along with the necessary dependencies.

```bash
pip install -r requirements.txt
```

## Usage
### Load the Model
```python
import pickle

# Load the trained model
rf_to_load = pickle.loads(saved)
```

### Make Predictions
```python
ind = rf.predict([
    [23.720338, 89.592641, 7.335604, 50.501694, 1032.378759],
    [27.879734, 46.489704, 5.952484, 4.990053, 992.614190],
    [25.069084, 83.072843, 1.371992, 14.855784, 1007.231620],
    [23.622080, 74.367758, 7.050551, 67.255282, 982.632013],
    [20.591370, 96.858822, 4.643921, 47.676444, 980.825142]
])
class_label = {1:'rain' , 0:'no rain'}
hrl = class_label.get(ind[0])
# hrl = [class_label.get(i) for i in ind[[0, 1, 2, 3, 4]]] for multiple predictions
hrl
```

## Model Details
- **Algorithm:** [Specify the ML algorithm, e.g., Random Forest]
- **Input Features:** [List the features used]
- **Output Classes:** Rain , No Rain
- **Training Data:** [Briefly describe dataset]

## Contributing
Feel free to fork this repository, make improvements, and submit a pull request.

## License
This project is licensed under the MIT License. See `LICENSE` for details.

