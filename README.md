# AI(fall detection)
This is the project for the 2023 "Advanced robotic ai" at hanyang university.

## Steps to run Code
### Clone the repository
```
git clone https://github.com/kyungmin0101/2023_advanced_robotic_ai
```

### Goto the cloned folder.
```
cd 2023_advanced_robotic_ai
```

### Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
- You can choose one as you prefer.
1. When you want to create a virtual environment(Recommended)
```
conda create -n robotics python=3.9
conda activate robotics
pip install --upgrade pip
pip install -r requirements.txt
```

2. When you want to use an already created conda virtual environment
```
###first of all, you have to enter your conda directory in the prefix field of robotics.yaml.

vi robotics.yaml
conda env create --file robotics.yaml
conda activate robotics
```

### Run the code with mentioned command below
#### for detection only
```
python fall_detection.py --video $your_video

### examples
python fall_detection.py --video examples/example_fall.gif
```

#### if you want to save your output
```
python fall_detection.py --video $your_video --save_output

### examples
python fall_detection.py --video examples/example_fall.gif --save_output
```
- Output file will be created in the original file exists

### Results
<table>
  <tr>
    <td>original video</td>
    <td>results</td>
  </tr>
  <tr>
    <td><img src="https://github.com/kyungmin0101/2023_advanced_robotic_ai/blob/master/examples/example_fall.gif"></td>
    <td><img src="https://github.com/kyungmin0101/2023_advanced_robotic_ai/blob/master/examples/examples_outexample_fall.gif"></td>
  </tr>
</table>
