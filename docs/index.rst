.. VDL documentation master file, created by
   sphinx-quickstart on Mon May 15 23:57:44 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

===============================
Welcome to VDL's documentation!
===============================

This documentation documents how to reproduce the result in the VDL project.

.. figure:: /img/architecture.png
    :width: 500px
    :align: center

    The architecture with multiple learners and multiple actors

The final presentation is hosted `here <https://docs.google.com/presentation/d/1r4zVv6bnImt8xTVtxopYhg1lWAeXrgliMfQQTo5Nlng/edit?usp=sharing>`__

Files in this project
=====================

.. code-block:: bash

    # Main
    docs/                   # Documentation files in reStructuredText format
    universe-starter-agent/ # Virtual distributed learning system, the code is
    # modified from https://github.com/openai/universe-starter-agent, which
    # provides the baseline learning algorithm.

    # Components
    learner-actor/          # Experiment code for learner-actor communication
    tensorflow_MNIST/       # Experiment code for P2P-multi-learner

    # Utility
    gym-demo/               # Virtual environnment demos to make sure the dev
    # boxs are correctly configured.
    benchmark/              # Benchmark code to evaluate the network speed and
    # speed of different virtual environments
    neonrace/               # Code to run trained neonrace auto-driving model
    spread/                 # Compiled spread and its python wrapper

    # Virtual arm
    arm-pose/               # Pose estimation code trained on the virtual arm
    # and test on the real arm.
    owi-arm/                # Code to control real and the virtual arm

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   multi_learner
   VDL
   virtual_arm
