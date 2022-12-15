# Reasonable Science Return

A ModuleManager configuration patch that changes science reward and transmission losses to make sense. Science experiments are put into three different categories:

| Category      | Reward | xmitDataScalar |
|---------------|--------|----------------|
| Sensor        | 100%   | 1.0            |
| Single sample | 100%   | 0.4            |
| Multi-sample  | 100%   | 0.2            |

Effectively, this means that experiments that are "Sensors" can be transmitted or returned, with no penalties for either -- it's just data! On the other hand, single sample experiments can't have their full science value transmitted; some of the sample must be examined back on Kerbin to obtain the full value. However, you do get a reasonable amount of science from transmitting, so it may still make sense to include it in a mission that won't return. Finally, multi-sample experiments need a lot of analysis back home, so you won't get very much science from just transmitting the recorded data.

You can see what category any given science part falls into by checking its description in the VAB or SPH.
