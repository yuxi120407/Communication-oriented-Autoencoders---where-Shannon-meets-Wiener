## Compare pri_AE and basic_AE for adding channel noise in the model
### pri_AE
We use one Gaussian distribution with zero mean and std is 5 in the bottleneck layer, the scale is 0.1, alapha is 0.1 and beta is 1. And then we add different SNR from 4dB to 18dB in the channel noise and calculate the mse in the end.

J = L(S, D(E(S))) + scale*(alapha*H(E(S)) + beta*Dcs(E(S)||P))
### basic_AE
we don't add anything in the loss function except for the mse between input and output.

### Results
| Channel Noise  | basic_AE  | pri_AE |
| :------------ |:---------------:| -----:|
| 4dB     | some wordy text | $1600 |
| 6dB      | centered        |   $12 |
| 8dB | are neat        |    $1 |
