## Compare pri_AE and basic_AE for adding channel noise in the model
### pri_AE (Pri_autoencoder)
We use one Gaussian distribution with zero mean and the standard deviation is 5 in the bottleneck layer, the scale is 0.1, alapha is 0.1 and beta is 1. And then we add different SNR from 4dB to 14dB in the channel noise and calculate the mse in the end.

J = L(S, D(E(S))) + scale*(alapha*H(E(S)) + beta*Dcs(E(S)||P))
### basic_AE (stack autoencoder)
we don't add anything in the loss function except for the mse between input and output.

### Results
| Channel Noise  | basic_AE  | pri_AE  |
| :------------  |:---------:| -------:|
|    4dB         | 0.0713    | 0.0592  |
|    6dB         | 0.0663    | 0.0549  |
|    8dB         | 0.0619    | 0.0516  |
|    10dB         | 0.0571   | 0.0490  |
|    12dB         | 0.0521    | 0.0469  |
|    14dB         | 0.0481    | 0.0454 |

