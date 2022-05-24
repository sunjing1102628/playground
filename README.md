# Playground

> First time? check out our [website](https://www.pommerman.com) for more information,
> our [Discord](https://discordapp.com/invite/wjVJEDc) to join the community,
> or read the [documentation](./docs) to get started.

Playground hosts Pommerman, a clone of Bomberman built for AI research. People from around the world submit agents that they've trained to play. We run regular competitions on our servers and report the results and replays.

There are three variants for which you can enter your agents to compete:

* FFA: Free For All where four agents enter and one leaves. It tests planning, tactics, and cunning. The board is fully observable.
* Team (The NIPS '18 Competition environment): 2v2 where two teams of agents enter and one team wins. It tests planning, and tactics, and cooperation. The board is partially observable.
* Team Radio: Like team in that a it's a 2v2 game. Differences are that the agents each have a radio that they can use to convey 2 words from a dictionary of size 8 each step.

This is a PyTorch starting point for experimenting with ideas for the Pommerman competitions;

The reinforcement learning codebase is based upon the Pommerman(https://github.com/MultiAgentLearning/playground)

* Pre-requisites


Python 3.6.0+ (including pip)
Docker (only needed for DockerAgent)
virtualenv (optional, for isolated Python environment)
* Installation

OPTIONAL: Setup an isolated virtual Python environment by running the following commands
$ virtualenv ~/venv
This environment needs to be activated for usage. Any package installations will now persist in this virtual environment folder only.

source ~/venv/bin/activate

* Clone the repository
$ git clone https://github.com/MultiAgentLearning/playground ~/playground
Install the pommerman package. This needs to be done every time the code is updated to get the latest modules
$ cd ~/playground
$ pip install -U .