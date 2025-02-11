# Expo Camera `onBarCodeScanned` unreliability

This repository demonstrates a bug in Expo's Camera API where the `onBarCodeScanned` prop's callback function does not always fire when a barcode is detected.  This leads to unpredictable behavior in barcode scanning applications.

## Bug Description

The `onBarCodeScanned` prop, intended to trigger a callback upon barcode detection, inconsistently fails to fire.  This occurs despite proper camera setup and clear barcode visibility within the camera's viewfinder.  This makes building reliable barcode scanning functionality challenging.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`. 
4. Point the camera at a barcode. Note that the callback might not always fire.

## Solution

The provided solution explores potential workarounds and improvements to mitigate the unreliability of the `onBarCodeScanned` prop. It involves implementing alternative barcode scanning libraries or strategies, or enhancing error handling to increase robustness.  More research may be needed to find a definitive solution. 