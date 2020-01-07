
# 433Mz Wireless Transmitter Receiver Module

<img src="img/433Mz RF Transmitter.jpg"
     alt="433Mz RF Transmitter"
     style="float: left; margin-right: 10px;" />

## Working

 **Transmitter Module** is the SAW resonator which is tuned for 433.xx MHz operation. When a logic HIGH is applied to the DATA input, the oscillator runs producing a constant RF output carrier wave at 433.xx MHz and when the DATA input is taken to logic LOW, the oscillator stops. This technique is known as Amplitude Shift Keying.

**Receiver Module** consists of a RF tuned circuit and a couple of OP Amps to amplify the received carrier wave from the transmitter. The amplified signal is further fed to a PLL (Phase Lock Loop) which enables the decoder to “lock” onto a stream of digital bits which gives better decoded output and noise immunity.

**Phase Lock Loop(PLL)** or phase-locked loop is a control system that generates an output signal whose phase is related to the phase of an input signal. There are several different types; the simplest is an electronic circuit consisting of a variable frequency oscillator and a phase detector in a feedback loop. The oscillator generates a periodic signal, and the phase detector compares the phase of that signal with the phase of the input periodic signal, adjusting the oscillator to keep the phases matched.

**Amplitude Shift Key(ASK)** is a form of amplitude modulation that represents digital data as variations in the amplitude of a carrier wave. In an ASK system, the binary symbol 1 is represented by transmitting a fixed-amplitude carrier wave and fixed frequency for a bit duration of T seconds. If the signal value is 1 then the carrier signal will be transmitted; otherwise, a signal value of 0 will be transmitted.

**Frequency-shift keying (FSK)** is a frequency modulation scheme in which digital information is transmitted through discrete frequency changes of a carrier signal. The technology is used for communication systems such as telemetry, weather balloon radiosondes, caller ID, garage door openers, and low frequency radio transmission in the VLF and ELF bands. The simplest FSK is binary FSK (BFSK). BFSK uses a pair of discrete frequencies to transmit binary (0s and 1s) information. With this scheme, the "1" is called the mark frequency and the "0" is called the space frequency.

## Specification
- Receiver frequency: 433MHz
- Receiver typical sensitivity: 105Dbm
- Receiver current supply: 3.5mA
- Receiver operating voltage: 5V
- Low power consumption
- Transmitter frequency range: 433.92MHz
- Transmitter supply voltage: 3V~6V
- Transmitter output power: 4~12Dbm

## Connections - Transmitter
- DATA (Rx & Tx) pin accepts digital data to be transmitted.
- VCC can be any positive DC voltage between 3.5V to 12V. Higher the Voltage, the greater the range will be.
- GND is a ground pin.

## Connections - Reciever
- Receiver VCC needs to be 5V.
- DATA (Rx & Tx) pins output the digital data received. 
- GND is a ground pin. 

## External library required for Arduino IDE
None

## Annotations
- **Vcc:** Positive Voltage 
- **GND:** Ground Negative 
- **Tx:** Transmitter Pin
- **Rx:** Reciever Pin

## References 
- <a href="https://en.wikipedia.org/wiki/Amplitude-shift_keying" target="_blank">Amplitude Shift Key (ASK)</a>
- <a href="https://en.wikipedia.org/wiki/Frequency-shift_keying" target="_blank">Frequency Shift Key (FSK)</a>
- <a href="https://en.wikipedia.org/wiki/Phase-locked_loop" target="_blank">Phase Loop Lock(PLL)</a>

---
#### Managed by [Contemplativeradicals](https://contemplativeradicals.com) 
##### for inconsistancies mail to: admin@contemplativeradicals.com