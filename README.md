# Reasonable Science Return

A ModuleManager configuration patch that changes science reward and transmission losses to make sense. Science experiments are put into three different categories:

- **Sensor** instruments:  100% *reward*, 1.0 `xmitDataScalar`
- **Single sample** instruments: 100% *reward*, 0.4 `xmitDataScalar`
- **Multi-sample** instruments: 100% *reward*, 0.2 `xmitDataScalar`

Effectively, this means that sensor experiments can be transmitted or returned, with no penalties for either -- it's just data! On the other hand, single sample experiments can't have their full science value transmitted; some of the sample must be examined back on Kerbin to obtain the full value. However, you do get a reasonable amount of science from transmitting, so it may still make sense to include it in a mission that won't return. Finally, multi-sample experiments need a lot of analysis back home, so you won't get very much science from just transmitting the recorded data.

You can see what category any given science part falls into by checking its description in the VAB or SPH.

Currently, science parts from stock as well as the following mods are supported:

- Far Future Technologies
- Kerbal Planetary Base Systems
- Station Parts Expansion Redux
