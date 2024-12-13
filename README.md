# React Native Dimensions API Intermittency Bug

This repository demonstrates a rare bug encountered when using the `Dimensions` API in React Native. The API occasionally returns incorrect screen dimensions, leading to unpredictable layout behavior.  The provided code showcases the problem and its solution.  The bug is challenging to reproduce consistently, making it particularly troublesome.

## How to reproduce (approximately):

While there's no guaranteed way to trigger this bug, it is most likely observed when the application is under heavy load or after a quick orientation change. The bug often appears and disappears seemingly randomly.

## Solution:

The solution involves adding logic to handle the edge case of incorrect dimensions, using a combination of timeout logic and fallback dimensions.