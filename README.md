# Data-Generation
Procedures to generate data for some AI benchmarks

For Megatron-LM, the generation of the training data will require reuse of NVidia's original BERT implementation data processing scripts.

Step 1. clone the DeepLearningExamples from NVidia
Step 2. cd into PyTorch/LanguageModeling/BERT
Step 3. build the container or just pull in my container `sudo docker pull lsetharak2020/bert`
Step 4. launch and enter the bert container and cd into the data folder
       `sudo bash scripts/docker/launch.sh`
       if you don't have any gpus, just remove the gpu lines from the launch script. Data processing will not take any gpus
       
Step 5. download books1 and books3 and the wiki corpus into the data folder
