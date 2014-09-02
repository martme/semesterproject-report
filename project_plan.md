# Project Plan

## Background

The background for this project is the work by Daniel Genkin, Adi Shamir and Eran Tromer presented in the paper titeled RSA Key Extraction via Low-Bandwidth Acoustic Cryptanalysis. As the title suggests, the authors managed to extract a full 4096 bit RSA key using acoustic noice as a side channel, giving a detailed expnanation of their approach in their work.

## Premises and Limitations

## Description of the problem

See problem description in separate document.

## Objectives of the work
Our objective is to verify that Low-Bandwidth Acoustic signals is indeed a viable side channel for use in cryptanalysis, and to reproduce the results from the original research team.

## Criteria for goal achievements

- Our initial goal is to distinguish between different CPU instructions such as `HLT`, `MUL` etc, by looking at the signal picked up from a microphone listening to the target computer.
- Our goal is to be able to extract a non-negligible amount of bits from the 4096 bit RSA key used by the target, with a significantly higher certainty than blind guessing.
- The ultimate goal is to extract a fill 4096 bit RSA key using the acoustic channel
- Extra credits: Use a mobile device as the microphone to mount the attack

## Uncertainty and risks

- Limited knowledge in lab setups and necessary equipment
- Our limited knowledge in C programming and signal processing.
- We might not observe a good enough signal-to-noice ratio for our attack to work

## Work plan

### Step 1
- Obtain sufficient background knowledge by studying the original reseach
- Implement the sound and signal processing mechanisms needed in C
- Implement way to visualize and analyze obtained data in real time

### Step 2
- Implement program to force loop of hardware instructions for observation
- Observe, analyze and identify signatures of the different instructions

### Step 3
- Setup attack prerequisite (computer running GnuPG 1.4.15 running Thunderbird with the EnigMail plugin)
- Implement the chosen plaintext procedure
- Implement the autoanalysis of the side channel information
- Improve attack




