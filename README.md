# Wi-Fi Attacks: Brute-Force & Fuzzing with Raspberry Pi

This repository contains two practical security exercises developed for the course *Mobile and Wireless Network Security* at the University of the Aegean. It includes:

- A brute-force login simulation against a router's admin panel using a **Raspberry Pi Pico W** as a USB HID device.
- A fuzzing campaign using **WPAxFuzz** to analyze the resilience of Wi-Fi management frames on Access Points and Stations.

---

## 🔒 Project 1: Brute-Force via Raspberry Pi Pico W

- Uses CircuitPython and `adafruit_hid` to simulate keyboard input.
- Performs login attempts via Chromium browser on a Linux machine.
- Sends successful credential pair to a remote server using `curl`.

📂 See folder: [`pico-bruteforce/`](./pico-bruteforce)

---

## 📡 Project 2: Wi-Fi Management Frame Fuzzing with WPAxFuzz

- Targets Beacon, Probe Request, Association Request/Response, and Authentication frames.
- Observed stability issues in STA devices and packet rejection behavior.
- Collected `.pcap` files and analyzed results with Wireshark.

📂 See folder: [`wpaxfuzz-fuzzing/`](./wpaxfuzz-fuzzing)

---

## 🧠 Threat Modeling

The project includes a threat model based on the **Security Cards framework**.

📄 See: [`threat-model.md`](./threat-model.md)

---

## 🧪 Tools & Requirements

- Raspberry Pi Pico W + CircuitPython
- WPAxFuzz, Aircrack-ng suite
- Wireshark, tshark
- Linux host machine with monitor mode-supported Wi-Fi adapter

---

## 📚 License

This repository is released for academic and research purposes. Always follow ethical hacking principles.
