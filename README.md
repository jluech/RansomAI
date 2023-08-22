# RansomAI
A Reinforcement Learning-based framework that can be integrated into existing ransomware samples to adapt their encryption behavior and stay stealthy while encrypting files.

`RansomAI` is introduced by [1].
However, the framework may also be referred to as ROAR (Ransomware Optimized with AI for Resource-constrained devices) as introduced by its corresponding master thesis [2].

It is generally advised to first consult the report of said master thesis.
The report motivates the thesis and introduces the required background.
It further explains the development, reasoning, and results of each prototype in great detail.

## Git Submodules

This repository contains two submodules:
1) `roar_server` with the RL Agent and command and control (C&C) part of ROAR
2) `roar_client` with the underlying ransomware of ROAR

Specifically, this is an umbrella repository which only points to a specific commit of the submodules.
If you commit any changes to a submodule, the umbrella repository will NOT automatically contain these changes.
To check for updates to the respective submodules, you can run the following command: `git submodule update --remote --merge`

Here are two useful links to familiarize yourself with git submodules:
- https://dev.to/milu_franz/git-explained-an-umbrella-structure-using-git-submodules-20dl
- https://git-scm.com/book/en/v2/Git-Tools-Submodules

# References
- [1] von der Assen, J., Celdrán, A. H., Luechinger, J., Sánchez, P. M. S., Bovet, G., Pérez, G. M., & Stiller, B. (2023). RansomAI: AI-powered Ransomware for Stealthy Encryption. arXiv preprint arXiv:2306.15559.
- [2] Lüchinger, J. (2023). AI-powered Ransomware to Optimize its Impact on IoT Spectrum Sensors. https://files.ifi.uzh.ch/CSG/staff/vonderassen/extern/theses/ma-luechinger.pdf. University of Zurich, Switzerland.
