- **Installation**
    
    ```bash
    conda create -n heat-hit python=3.11 -y
    conda activate heat-hit
    
    cd heat-hit/yolov13
    pip install -r requirements.txt
    pip install -e .
    ```
    
- **Training**
    
    ```bash
    # Data Preparation: Absolute path needs to be corrected
    cd heat-hit/yolov13
    source ./setup_env.sh
    ```
    
    ```bash
    yolo cfg=configs/train.yaml
    ```
    
- **Test**
    
    ```bash
    yolo cfg=configs/val.yaml
    ```
    
- **Inference**
    
    ```bash
    yolo cfg=configs/predict.yaml
    ```
