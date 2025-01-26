# Expo CLI Metro Bundler Random Crashes

This repository demonstrates a bug encountered with the Expo CLI's Metro bundler, where the bundler would crash randomly during development without providing any error messages.  The issue significantly disrupted the development workflow due to its unpredictable nature. The solution implemented explores a potential workaround to mitigate this problem. 

## Bug Description
The Expo Metro bundler would occasionally terminate unexpectedly during development, offering no helpful logs or error messages to indicate the cause. This made it difficult to identify and address the root problem.

## Reproduction Steps
The exact conditions that triggered the crash were not consistently reproducible.  It seemed to occur at random during various operations like starting the development server, making code changes, or simply letting the app idle. 

## Solution
While the underlying cause of these crashes couldn't be definitively identified, a potential solution involved checking the system resources (memory and CPU usage).  If these were close to capacity, it may contribute to the Metro bundler instability. By optimizing project dependencies and ensuring adequate system resources, the frequency of these crashes appeared to decrease. The code provided demonstrates a basic implementation of monitoring system resource usage in the context of an Expo application. Although not a permanent fix, this solution provides a way to monitor system resources to potentially prevent these crashes.