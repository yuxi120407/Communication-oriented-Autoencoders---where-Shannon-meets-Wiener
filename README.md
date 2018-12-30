# Communication-oriented-Autoencoders---where-Shannon-meets Wiener
the python codes of paper "Communication-oriented Autoencoders - where Shannon meetsWiener"


### Installation
1. Install an Anaconda environment (recommended).
2. From the environment, update Theano: `conda uninstall theano; pip install https://github.com/Theano/Theano.git`
3. Install Keras: `pip install https://github.com/fchollet/keras.git@52f48e1f462090db19b03ae11dce`
4. Install Seya: `pip install git+https://github.com/EderSantana/Seya.git`
5. Install agnez: `pip install git+https://github.com/AgnezIO/agnez.git`
6. Install seaborn: `pip install seaborn`

### Demo
1. we upload demos which we train autoencoder architecture with Pri and c-loss funciton. 
2. we train four digitals: '0','1','4','5' with four Gaussian prior and show the bottleneck layer, which is shown in 'C-Pri-AE-four    Gaussian prior demo'. We also add source noise when training, add channel noise when testing and calculate mean square error which is shown in 'C-Pri-AE-ten Gaussian prior demo'. The weights which we have already trained are in 'noise_Gaussian4_pri model' and 'noise_Gaussian10_pri model'

### Pri and C-loss
1. The implementation of principle of relevant information(Pri) function shown in the equation(11) is in 'regularization.py'
2. the codes of C-loss objective funciton are in 'objectives.py'
