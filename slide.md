[//]: # "slide Markdown for remark"

class: center, middle

# IoT Platforms for STEM Education

???
Speaker notes
_Markdown_ also available here

---

# Agenda

- [Introduction](#intro)
- [Project Ideas](#ideas)

---

class: center, middle
name: intro

# Introduction

---

# Physical Programming and IoT

- _Physical Programming_
  - system embedded with electronics, software, sensors, actuators
  - integrates the physical world into computer-based systems
- _Internet of Things_
  - Physical Programming with network connectivity
  - LAN or WAN or WAN through gateway

.footnote[
Being an embedded system engineer for more than 10 years, all these are fancy terms for embedded system programming.
]

---

# Hardware

- SBC (Single Board Computer)
  - Rasberry Pi (_Broadcom BCM series_)
  - Asus Tinker Board (_Rockchip RK3288_)
  - Banana Pi (_AllWinner series_)
  - ...
- Micro Controller
  - Arduino (_Atmel series_)
  - Micro:bit (_Nordic_ + _NXP nRF51822_)
  - _ESP32_
  - _STM32 series_
  - ...

.footnote[
Chipsets are in *Italics*; a product may use different chipsets
]

---

# Single Board Computer

- general purpose computer like your desktop  
  just slower and less compatible
- larger form factor (than micro controller), with HDMI output
- usually runs Linux OS
- usually not using x86 processors
- usually have built-in connectivity (Bluetooth + WiFi)
- can install software packages, including compilers and interpreters
- code within the board
- can drive micro controllers and other modules over serial(UART)/SPI/I²C
- have native interface for display and camera

.footnote[
Some products also run Android to target end-users
]

---

# Micro Controller

- usually runs RTOS (Real Time OS)
- with interrupts to provide real-time response
- better for interacting with other modules
  - more IO pins
  - more PWM (pause width modulator, mimics analog signal)
  - usually with ADC and DAC (analog <> digital converter)
- code in host PC, compile and flash executable to memory
- usually requires other modules to provide connectivity

---

# Programming Environment

- Block programming
  - intuitive programming environment for kids
  - no syntax error, discoverable APIs
  - [Scratch](https://scratch.mit.edu/) itself is open source
  - ported to support various micro controllers
  - examples:  
    S4A (Arduino boards), mblock (Makeblock), [makecode](https://makecode.microbit.org/) (Micro:bit)
  - limited support for external modules  
    may need to acquire modules from the specific vendor
  - can converts to interpreted language (depends on vendor)  
    e.g.: JavaScript, Python

---

# Programming Environment

- Arduino IDE
  - supports official Arduino boards  
    and many other micro controllers + code in C language + not suitable for small kids
- Python
  - easy to learn and good for further advancement in programming
  - native CPython on SBC
  - [PyMite](https://wiki.python.org/moin/PyMite) and [MicroPython](https://micropython.org/) for micro controllers
  - [Micro:bit - Python editor](https://python.microbit.org/v/1)
  - not recommended for micro controllers
  - limited features, old Python version
  - chipset support is limited
  - unless well supported, like Micro:bit

---

# Makeblock's mBot

- mBot's core is a Arduino Uno board
- uses RJ25 as connectors
- more expensive module and peripherals
- cheaper alternatives at Taobao ~¥300

---

# CocoRobo

- Arduino plus custom made boards
- also 3D printed parts
- [COCOROBO 課程中心](https://cocorobo.hk/online/curriculumKit/0)

---

# Micro:bit

- many built-in components + buttons + 5x5 LED dot matrix + Bluetooth and radio + temperature and light sensor + accelerometer and magnetometer (compass)
- vibrant community and ecosystem of peripherals
- peripherals are a little bit expensive
- main board is actually not expensive  
  considering all the built-in components, built quality and vendor support
- can do much more with extension board  
  can use all of Arduino modules
  it's in essence a micro-controller system
- [Projects - Microsoft MakeCode](https://makecode.microbit.org/projects)

---

class: center, middle
name: ideas

# Project Ideas

---

# Forewords

- most micro controller will work as long as they have IO pins for ADC/DAC and PWM
- we can add external components if ADC/DAC is not enough or absent (for SBC)
- we will use bread board and Dupont cables
- low voltage components (3.3V-5V, 9V and 12V sparingly), use battery for power

---

# Goals

> to be discussed

- learn programming
- interact with real world through software you wrote
- fun
- practical application  
  learn how everyday products are made
- external competition
- improve English skills  
  teaches in English  
  require students to write comments for code  
  improve written skill as well
- [Intro to CS - Microsoft MakeCode](https://makecode.microbit.org/courses/csintro)

---

# Basic Electronics

- Voltage and Current
- AC and DC  
  which is used where, benefits
- Analog and Digital  
  binary number
- Magnetism  
  play with compass
- Electro-magnetic Induction  
  to explain noise in electric circuit
- Pull-up and Pull-down resistor  
  for input signals  
  demo with two kids holding a string as voltage level

---

# GPIO

- connect to external sensors
- teaches electronics
- with extension board, crocodile clip and breadboard

---

# micro:bit sensors

- buttons
- dot matrix
- temperature
- light sensor
- accelerometer
- magnetometer (compass)
- Bluetooth and radio

---

class: center, middle

# .red[♥] Thanks all .red[♥]

## Q & A
