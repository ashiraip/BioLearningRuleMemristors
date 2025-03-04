# BioLearningRuleMemristors

This folder is sorted into three subfolders:

Basic Setup
- memristor_slow_1.sub
  LTspice Implementation of model
- memristor_with_state.asy
  symbol for memristor from Yakopcic, C. et. al. 2012
- SlowTimeCharacterisation_recreate_ExperimentData.asc
  recreated circuit from experimental data collection

Associative Learning Circuit
- learn_pulse_reset_pythonIn.asc
  The associative learning circuit as implemented in LTspice
  The circuit takes in specific inputs from the following files:
  - v_a_ascc_l
  - v_b_ascc_l
  - s_l_ascc_l
  The circuit also requires the first 2 files from "Basic Setup" to run successfully
- Hardware_Test_Results.zip
  Recordings on hardware done by Jimenez-Olalla, N. for the associative learning circuit
  Note: the hardware vs simulation results were obtained by taking the data for Va, Vb, and Learning
  from each hardware recording and feeding it to the LTspice simulation

XOR Circuit
- working_XOR_connect_realMLP.asc
  The non-linear learning circuit as implemented in LTspice
  The circuit takes in specific inputs from the following files:
  - v_a_binary
  - v_b_binary
  - s_l_binary
  The circuit also requires the first 2 files from "Basic Setup" to run successfully
