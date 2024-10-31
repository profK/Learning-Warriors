# Learning-Warriors
The learning warriors  project is an attempt to use a runtime-learning Feed Forward Multilayer Perceptron to teach creatrues to fight within UE5

## PLugins
There are 3 custom plugins that we wrote for this project:

### NNEBlueprintInterface
https://github.com/profK/NNEBlueprintInterface

This exposes a set of functiosn for using the UE5 Neural network Engine from blueprints.
It supports creating models from either ONNX files on disc or in memory.
It has a number of limitations:
(1) It only supports 1D Tensors for input and output
(2) It only supports the NNERuntimeORT NNE engine implementation

### ONNXBuilderPlugins
https://github.com/profK/ONNXBuilderPlugins

This is a set of plugins that allow you to build ONNX descriptions of feed foward multi-layer perceptrons in
memory and reset their node weights as needed. The binary form of these models can be extracted and sent to the
NNEBlueprintInterface plugin to be turned into NNE Models

### GeneticTrainerBPL
https://github.com/profK/GeneticTrainerBPL

This is a blueprint library for evolving scored sets of parameters expressed as a genome of floating point genes

### Linear-Equation-MLP-Test-Content
https://github.com/profK/Linear-Equation-MLP-Test-Content

This is the Content (specifically the Blueprints) for a test UE project that uses genetic learnning to teach a
feed foward multi-layer-perceptron how to calculate a 1D linear equation with a known mean and dev.

### Demo project
https://drive.google.com/file/d/1nK9_wSP2rjIpEgjr5aG4h7qkNb3nAtSW/view?usp=sharing
All of the above can be downloaded in a pre-integrated project at the above link
