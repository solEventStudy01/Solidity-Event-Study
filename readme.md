# Solidity-Event-Logging-Study

## What is this repository? 

This repository serves as the replication package for our ESEC/FSE 2023 submission **"Understanding Solidity Event Logging Practices in the Wild"**. 

Writing logging messages is a well-established conventional programming practice, and it plays an extremely important role in various software development activities. The logging mechanism in Solidity programming is enabled by the high-level `event` feature, but so far there have been no study for understanding Solidity event logging practices in the wild. We make the first attempt to provide a quantitative characteristic study of the current Solidity event logging practices using 2,915 Solidity projects hosted on Github. Our study systematically investigates the pervasiveness of event logging, the goodness of current event logging practice, and in particular the evolution of event logging code, and generates 8 novel and important findings. We also present the implications of our findings, which shed light for developers, researchers, tool builders, and language designers to improve the practice of event logging. To demonstrate the potential benefits of our findings, we develop a simple checker based on one of our findings and effectively detect problematic event logging code in 35 popular GitHub projects and 10 project owners have already confirmed the issues detected by us.

This repository contains the collected large scale data about density of event logging code, evolution of event logging code in particular our manual analysis of the characteristics of independent event logging code modifications, and our tool for checking problematic event logging parameter in order to save gas.

## Structure of this repository

The repository contains three folders: Event-Density, Event-Evolution, and Event-Checker.

- [Event-Density](./Event-Density) contains the raw data about event use per project and per LOC (lines of code) for each of the studied 2,915 Solidity projects. 
- [Event-Evolution](./Event-Evolution) contains the snippets of the original event logging code changes for 419 independent event logging code modifications and our manual analysis of the categories and reasons for these modification.
- [Event-Checker](./Event-Checker) contains the source code for the tool and the instructions on how to install and use the tool. 

Inside each folder, we give more detailed descriptions of the content it contains.  


