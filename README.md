# Cache Memory Simulator: Reducing Conflict Misses

# Introduction
This project involves simulating a cache memory system using champsim to understand cache misses and propose solutions to reduce conflict misses. The main objective is to improve the hit rate, thereby enhancing the Average Memory Access Time (AMAT), Instruction Per Cycle (IPC), and overall performance.

# Problem Statement
Given a fixed configuration of the last level cache (2MB, 16 ways, 64 byte block size), the goal is to find a suitable remapping of addresses to cache lines to reduce conflict misses. Conflict misses occur when multiple addresses map to the same cache set, leading to under-utilization of some sets and over-utilization of others.

# Proposed Solution
The traditional method of mapping addresses to cache lines using the modulo operator can result in inefficient cache utilization. To address this, we implemented a remapping strategy by classifying cache sets into "hot sets" and "cold sets":

Hot Sets: Cache sets with high access rates.
Cold Sets: Cache sets with low access rates.
By remapping addresses from hot sets to cold sets, we aim to balance the load across the cache, thereby reducing conflict misses and improving cache efficiency.

# Results
The proposed remapping strategy significantly reduces conflict misses, resulting in improved hit rates, lower AMAT, and increased IPC. Detailed performance metrics can be found in the results directory.

# Contact
For any queries or contributions, please contact:

Name: Saaransh Sharma
GitHub: saar4nsh
