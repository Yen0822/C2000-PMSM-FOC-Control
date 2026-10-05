# C2000 PMSM FOC Control

PMSM field-oriented control implementation using the TI TMS320F28379D.

## Features

- TI TMS320F28379D
- 10 kHz switching/control frequency
- ADC current sampling
- ePWM three-phase PWM generation
- eQEP encoder position/speed feedback
- PI speed and current control
- Clarke/Park coordinate transformation
- Inverse Park transformation
- SVPWM
- Bidirectional motor control

## Control Flow

`ADC current sampling -> Clarke/Park -> Id/Iq current control -> Vd/Vq -> Inverse Park -> SVPWM -> ePWM -> inverter -> PMSM`

Encoder feedback is acquired through eQEP for rotor position and speed feedback.

## Development Environment

- TI Code Composer Studio (CCS)
- TI C2000 TMS320F28379D
- C

## Notes

This repository contains an academic PMSM motor-control implementation developed for coursework/research practice. TI device-support files are retained to preserve the original CCS project structure.
