# Communication-oriented-Autoencoders---where-Shannon-meets Wiener
The python codes of paper "Communication-oriented Autoencoders - where Shannon meets Wiener"


### Installation
1. Install an Anaconda environment (recommended).
2. From the environment, update Theano: `pip install Theano==0.8.0`
3. Install Keras: `pip install keras==0.3.3`
4. Install Seya: `pip install git+https://github.com/EderSantana/Seya.git`
5. Install agnez: `pip install git+https://github.com/AgnezIO/agnez.git`
6. Install seaborn: `pip install seaborn`
7. Install hdf5: `pip install h5py `

### Demo
1. We upload demos which we train autoencoder architecture with Pri and c-loss funciton. 
2. We train four digitals: '0','1','4','5' with four Gaussian prior and visualize the bottleneck layer, which is shown in 'C-Pri-AE-four    Gaussian prior demo'. We also add source noise when training, add channel noise when testing and calculate mean square error which is shown in 'C-Pri-AE-ten Gaussian prior demo'. The weights which we have already trained are in 'noise_Gaussian4_pri model' and 'noise_Gaussian10_pri model'

### Pri and C-loss
1. The implementation of principle of relevant information(Pri) function shown in the equation(11) is in 'regularization.py'
2. The codes of C-loss objective funciton are in 'objectives.py'
