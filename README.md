# Reading-Notes
You are what you read, here are mine

### Notes taken from [Demystifying Entropy](https://towardsdatascience.com/demystifying-entropy-f2c3221e2550), [Demystifying Cross-Entropy](https://towardsdatascience.com/demystifying-cross-entropy-e80e3ad54a8?ZGa=true) and [Demystifying KL Divergence](https://towardsdatascience.com/demystifying-kl-divergence-7ebe4317ee68)

> Shannon defind the entropy as the smallest possible average size of lossless encoding of the messages sent from the soruce to the destination.

In general, when we need N different values expressed in bits, we need `$\log_2N$` bits and we don't need more than this. 

If a message type happens 1 out of N times, the above formula gives the minimum size required. 

```math
log_2N = -log_21/N = -log_2P
```

Combining with the probabilities to get the average size, we will get:

```math
Entropy = -\sum_iP(i)log_2P(i)
```

If Entropy is high, the **average encoding size** is significant which means each message tends to have more information. It is why high entropy is associated with disorder, uncertainty, surprise, unpredictability, amount of information.
