# Guess number

## Table of Contents

1. [observation](#observation)
2. [score_game](#score_game)
3. [random_predict](#random_predict)
4. [game_core_v2](#game_core_v2)
5. [game_core_v3](#game_core_v3)

## observation

The main task of the code is to benchmark and evaluate the performance of different number-guessing algorithms, specifically comparing the efficiency of various methods in terms of the number of attempts required to guess a randomly chosen number between 1 and 100.

## score_game

Benchmarking (in score_game):
The score_game function simulates running the guessing algorithm 10,000 times. For each trial, a random number between 1 and 100 is chosen, and the guessing algorithm (random_predict, game_core_v2, game_core_v3) is used to try and guess it. The average number of attempts across all 10,000 simulations is calculated and printed. This serves to assess the overall performance of the guessing algorithm.

Purpose:
The purpose is to determine the average number of attempts required for a random number-guessing algorithm (game_core_v2) to correctly guess a number in a range of 1 to 100. The overall goal is to understand how many attempts (on average) it will take for the algorithm to guess correctly, which helps evaluate its efficiency. This could be compared to other algorithms, such as binary search (game_core_v3), which would take fewer attempts.

## random_predict

The random_predict function you provided is designed to guess a number by generating random guesses from 1 to 100 without using any feedback (like whether the guess is too high or too low). The function keeps guessing until it finds the correct number and returns the number of attempts it took.

## game_core_v2

The function game_core_v2 that you've written follows a very simple logic for guessing a number. It starts by randomly picking a number between 1 and 100, and then gradually adjusts the guess by incrementing or decrementing it depending on whether the target number is higher or lower. Let's break down the code and discuss its functionality and performance.

## game_core_v3

This is the actual guessing algorithm. It uses binary search logic to guess a number. It starts by randomly selecting a number between 1 and 100 (predict). Then it compares the guess (predict) to the target number (number). Depending on whether predict is too high or too low, it narrows down the range for the next guess. The algorithm repeats this process until it correctly guesses the number. It returns the number of attempts required to guess the correct number.
