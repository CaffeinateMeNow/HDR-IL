

# Deep Imitation Learning for Bimanual Robotic Manipulation


This repository is for the NeurIPS 2020 paper "Deep Imitation Learning for Bimanual Robotic Manipulation" (https://papers.nips.cc/paper/2020/file/18a010d2a9813e91907ce88cd9143fdf-Paper.pdf). We present a deep imitation learning framework for robotic bimanual manipulation in a continuous state-action space. Our model learns to imitate table lifting movements in simulation and generalize the learned skills to tables at different locations.

The repository contains the files we used to generate our training data using and the models we used to obtain our experiment results. We used Pybullet to generate our simulations and Pytorch to build our deep learning models. More details are found below.


# Demonstrations
We created the following tasks in PyBullet to generate training data. The GIFs below are one instance of our demonstration for each of the two tasks. A video file showing our model predictions can be found in "Simulations.mov"

### Table Lifting Task Demonstration                                               

![](https://github.com/Rose-STL-Lab/HDR-IL/blob/master/table_lift.gif)       

### Peg-In-Hole Task Demonstration  

![](https://github.com/Rose-STL-Lab/HDR-IL/blob/master/ped_in_hole.gif)      




# Generating Data

All code for generating training data is found in the "Simulation Code" folder. Simulations are built up using low-level primitives such as lift or push. All simulations are written using the PyBullet physics engine. All components in the simulations are built-up using URDF files. These files can be easily extended to create other objects/tasks to be used in simulations. In order to save time, simulations are best run on a workstation with a GPU.

# Prediction Models
The prediction models are titled "Table_Lift_HDR-IL" for the table lifting task. Details about training the model can be found in "Model_Readme.txt"

# Citation
To cite our work:

@misc{xie2020deep,
      title={Deep Imitation Learning for Bimanual Robotic Manipulation}, 
      author={Fan Xie and Alexander Chowdhury and M. Clara De Paolis Kaluza and Linfeng Zhao and Lawson L. S. Wong and Rose Yu},
      year={2020},
      eprint={2010.05134},
      archivePrefix={arXiv},
      primaryClass={cs.RO}
}


# Authors

Fan Xie,
Alex Chowdhury








