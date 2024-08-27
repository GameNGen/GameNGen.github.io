# GameNGen

We present GameNGen, the first game engine powered entirely by a neural model
that enables real-time interaction with a complex environment over long trajectories at high quality.
GameNGen can interactively simulate the classic game DOOM at over 20 frames per second on a single
TPU. GameNGen simulations do not suffer from accumulated deterioration even after long play sessions,
achieving a PSNR of 29.4, comparable to lossy JPEG compression.
Human raters are only slightly better than random chance at distinguishing short clips of the game
from clips of the simulation.
GameNGen is trained in two phases:
(1) an RL-agent learns to play the game and the training sessions are recorded, and
(2) a diffusion model is trained to produce the next frame, conditioned on the sequence of past frames and
actions. Conditioning augmentations enable stable auto-regressive generation over long trajectories.

## Acknowledgments
This page was built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template) which was adopted from the [Nerfies](https://nerfies.github.io) project page.
